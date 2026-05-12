# Text-to-CAD Environment

> **Source:** [[Home|Wiki Home]] · [[Build-System]] · `5-Applications/text-to-cad/README.md` · `5-Applications/text-to-cad/AGENTS.md`

The Text-to-CAD harness (`5-Applications/text-to-cad/`) drives agentic 3D
modeling by exposing `build123d` and `OCP` (OpenCascade) bindings to coding
agents like Codex and Claude Code. This page documents the wiki-level view of
the standardized environment that supports the harness, including the VSCode
tasks and npm scripts that bootstrap the local virtual environment.

For the agent contract (file-targeted skills, viewer handoff rules, prompt-ref
grammar), see `5-Applications/text-to-cad/AGENTS.md`.

---

## CAD Environment Setup

The Text-to-CAD harness uses a repo-local virtual environment at
`5-Applications/text-to-cad/.venv` that is created from the pinned Python
interpreter described in [[Build-System#Python Environment Management]].

### VSCode Tasks (`.vscode/tasks.json`)

Three tasks bootstrap and validate the CAD environment from the VSCode
command palette (`Tasks: Run Task`):

| Task label | Action | Effect |
|---|---|---|
| `Install Python 3.11.15` | `uv python install 3.11.15` | Installs the pinned interpreter required by `build123d` / `OCP` |
| `Setup CAD Environment` | `python3.11 -m venv .venv && ./.venv/bin/pip install -r requirements-cad.txt` (cwd: `5-Applications/text-to-cad/`) | Creates `5-Applications/text-to-cad/.venv` and installs CAD dependencies |
| `Verify CAD Dependencies` | `./.venv/bin/python -c "import build123d; import OCP; print('CAD dependencies OK')"` | Confirms that `build123d` and `OCP` resolve inside the venv |

### NPM Scripts (`package.json`)

The same three operations are exposed as npm scripts at the repository root so
they can be invoked from CI, headless shells, or non-VSCode editors:

| Script | Equivalent action |
|---|---|
| `npm run install-python` | Install Python 3.11.15 via `uv` |
| `npm run setup-cad-env` | Create the text-to-cad venv and install `requirements-cad.txt` |
| `npm run verify-cad` | Re-run the `build123d` / `OCP` import check |

### Bootstrap order

```bash
# 1. From the repository root
npm run install-python       # uv python install 3.11.15
npm run setup-cad-env        # creates 5-Applications/text-to-cad/.venv
npm run verify-cad           # prints "CAD dependencies OK" on success
```

The `Setup CAD Environment` task is idempotent — re-running it against an
existing `.venv` will reuse it and only update pinned packages. To force a
clean rebuild, remove `5-Applications/text-to-cad/.venv` first.

### Agent contract

The harness's `AGENTS.md` requires all CAD tooling to be invoked through
`./.venv/bin/python` from `5-Applications/text-to-cad/`. The `Verify CAD
Dependencies` task is the canonical preflight check before running any of the
skill scripts (`gen_step_part`, `gen_step_assembly`, `gen_urdf`, `cadref`,
`snapshot`). If the verification fails, agents are expected to re-run the
`Setup CAD Environment` task before attempting CAD generation.

---

## Related

- [[Build-System]] — Python version pinning, uv integration, VSCode interpreter
  configuration that this environment builds on.
- `5-Applications/text-to-cad/README.md` — user-facing quick start, feature
  list, and bundled skill catalog.
- `5-Applications/text-to-cad/AGENTS.md` — agent contract, viewer handoff
  rules, and common harness commands.
- `5-Applications/text-to-cad/requirements-cad.txt` — pinned CAD dependency
  set installed into `.venv`.
