# Build System

> **Source:** [[Home|Wiki Home]] · [[../GETTING_STARTED.md|Getting Started]] · [[../CONTRIBUTING.md|Contributing]]

This page documents the build-system surfaces of the Sovereign Research Stack
that supplement the Lean toolchain described in `GETTING_STARTED.md`. Content
here is the wiki-level companion to the top-level setup docs and to the
VSCode tasks and npm scripts committed under the repository root.

---

## Python Environment Management

The repository pins a single Python version for all Python-based harnesses
(swarm scripts, CAD tooling, DeepSeek review adapters, etc.) so that
deterministic re-runs and AI-assisted review receipts remain reproducible.

| Surface | Value | Source |
|---|---|---|
| Python version | `3.11.15` | `.python-version` |
| Installer | `uv` (Astral) | VSCode task `Install Python 3.11.15`, npm script `install-python` |
| Interpreter path | `~/.local/share/uv/python/cpython-3.11-linux-x86_64-gnu/bin/python3.11` | `.vscode/settings.json` (`python.defaultInterpreterPath`) |

### Why a pinned `.python-version`

- `build123d` and `OCP` (the CAD stack used by `5-Applications/text-to-cad/`)
  publish wheels for CPython 3.11 only.
- DeepSeek review receipts (see [[DeepSeek-Review-Process]]) record SHA-256
  hashes of prompts and answers; differing Python runtimes can change tokenizer
  output and break receipt reproducibility for downstream review continuation.
- The Lean toolchain is independent of Python, but every Python harness must
  agree on a single interpreter so that artifacts produced by one stage
  (e.g. equation-forest extraction) can be re-validated by another stage
  (e.g. metaprobe replay) without environment drift.

### UV integration

`uv` is used as the installer for the pinned interpreter. The repository does
not bundle a `pyproject.toml` at the root — `uv` is invoked only to install
the interpreter itself, and per-application virtual environments are created
from that interpreter.

```bash
# Install the pinned interpreter (idempotent)
uv python install 3.11.15

# Equivalent npm shortcut from the repo root
npm run install-python
```

### VSCode integration

`.vscode/settings.json` sets `python.defaultInterpreterPath` to the
uv-managed CPython 3.11.15 binary. Open the repository in VSCode after the
interpreter is installed and the Python extension will resolve linting,
type-checking, and run/debug actions against the same interpreter used by
the npm scripts and VSCode tasks below.

If your `uv` install path differs (e.g. macOS or a non-default `XDG_DATA_HOME`),
override `python.defaultInterpreterPath` in your user-level settings rather
than editing the workspace setting — the workspace path is the source of
truth for receipt-bearing runs.

### Installation flow

```bash
# 1. Install uv itself (one-time, see https://docs.astral.sh/uv/)
curl -LsSf https://astral.sh/uv/install.sh | sh

# 2. Install the pinned interpreter
uv python install 3.11.15      # or: npm run install-python

# 3. (CAD only) Create the text-to-cad venv
npm run setup-cad-env          # see [[Text-to-CAD-Environment]]

# 4. (CAD only) Verify the CAD venv resolves build123d and OCP
npm run verify-cad
```

---

## NPM Script Surface (repo root `package.json`)

The repository root `package.json` exposes a small set of orchestration scripts
that wrap the VSCode tasks so that they are available outside the editor (CI,
remote shells, headless installs).

| Script | Wraps | Purpose |
|---|---|---|
| `npm run install-python` | `uv python install 3.11.15` | Install the pinned interpreter via uv |
| `npm run setup-cad-env` | `python3.11 -m venv` + `pip install -r requirements-cad.txt` in `5-Applications/text-to-cad/` | Create the text-to-cad virtual environment |
| `npm run verify-cad` | `import build123d; import OCP` in the text-to-cad venv | Validate that the CAD dependencies are importable |

See [[Text-to-CAD-Environment]] for the CAD-specific workflow these scripts
support.

---

## VSCode Tasks (`.vscode/tasks.json`)

The same three operations are exposed as VSCode tasks so they can be invoked
from the command palette (`Tasks: Run Task`) without leaving the editor.

| Task label | Equivalent npm script | Notes |
|---|---|---|
| `Install Python 3.11.15` | `npm run install-python` | Runs `uv python install 3.11.15` from the workspace root |
| `Setup CAD Environment` | `npm run setup-cad-env` | Creates `5-Applications/text-to-cad/.venv` and installs `requirements-cad.txt` |
| `Verify CAD Dependencies` | `npm run verify-cad` | Runs `./.venv/bin/python -c "import build123d; import OCP; print('CAD dependencies OK')"` from the text-to-cad directory |

Tasks present output in a shared panel so the install logs are persisted across
re-runs.

---

## Related

- [[Text-to-CAD-Environment]] — CAD-specific environment, requirements, and
  the agent contract that consumes `5-Applications/text-to-cad/.venv`.
- [[DeepSeek-Review-Process]] — receipt schema and review workflow that
  depends on the pinned Python interpreter for prompt-hash reproducibility.
- `GETTING_STARTED.md` — Lean toolchain installation and end-to-end build
  walkthrough for the Lean core.
