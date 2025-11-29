## Quick orientation

This repository is a very small exercise project (see `README.md`: "Proyecto de prueba para Estructura de Datos 2"). There are no build scripts, package manifests, or tests present. Treat this as a lightweight student/assignment repo: additions should be simple, self-contained, and clearly documented.

## What an AI agent should assume and confirm
- Assume language/runtime is unspecified. Before adding runnable code, ask which language/tooling the user prefers (Python, Java, C#, etc.).
- Assume minimal structure: add code under `src/` and tests under `tests/` unless the user requests otherwise.

## Recommended structure and conventions (discoverable + conservative)
- Source files: create `src/` at repo root. Use clear filenames, e.g. `src/problem_<n>.<ext>`.
- Tests: place in `tests/` and use the common test runner for the language chosen (pytest, JUnit, etc.). Include a brief README entry when adding test commands.
- Documentation: update `README.md` whenever you add build or run steps. Keep the top-level README as the canonical quick-start.

## Developer workflows (what to document and ask the user)
- If you add a build or dependency file (e.g., `package.json`, `requirements.txt`, `pyproject.toml`, `pom.xml`), immediately update `README.md` with exact commands to set up, build, and run tests.
- If you need to run commands locally, request the user's preferred shell/OS. (This workspace runs on Windows by default.)

## Examples for common edits
- Adding a Python solution:
  - Create `src/solution_x.py` and `tests/test_solution_x.py` (pytest).
  - Update `README.md` with:
    - how to create a venv, install (`pip install -r requirements.txt`), and run tests (`pytest`).

- Adding a compiled-language solution (e.g., Java/C#):
  - Add a minimal project structure (`src/`, `tests/`) and a build manifest. Document exact `dotnet`/`mvn`/`gradle` commands in `README.md`.

## Integration points & external dependencies
- No external services or APIs are present in the repo. If you add integrations, declare them in `README.md` and include credentials/instruction notes only if the user provides them (do not hard-code secrets).

## Examples of project-specific patterns to follow
- Keep changes minimal and self-contained: this repo appears to be for exercises, so prefer small commits that implement one problem/feature and include a test.
- Use Spanish or bilingual comments when the surrounding documentation is Spanish; keep code identifiers in English for broader readability.

## When you can't proceed
- If essential information is missing (target language, test runner, expected input/output formats), stop and ask the user for that detail before implementing.

## Final checklist for PRs
- Update `README.md` with setup/run/test commands.
- Include tests demonstrating intended behavior.
- Provide a 1–2 line PR description explaining files added and how to run them.

If any of the above assumptions are incorrect, tell me which parts you want changed or provide the missing project details (language/runtime, testing preference, and any sample input/output). I'll update this file accordingly.
