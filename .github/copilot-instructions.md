# Copilot instructions for this repository

## Project snapshot

This repository is intentionally minimal: it is a GitHub profile-style repository with a short profile README and a tiny Python script. There is no application framework, package manager configuration, or test harness in the repo today.

## Build, test, and lint commands

There are no formal build, lint, or test scripts configured for this repo.

Use the script directly:

```bash
python main/tmp.py
```

For a quick syntax check:

```bash
python -m py_compile main/tmp.py
```

If this repository grows into a larger Python project later, add the project’s real commands at that time; for now, the working validation path is to run the script directly or compile it for syntax validation.

## High-level architecture

The repo is effectively two pieces:

- `README.md`: GitHub profile content used for the repository landing page.
- `main/tmp.py`: the only executable code in the repo, a small standalone Python script that prints a greeting and a short list of interests.

There are no modules, services, packages, or runtime boundaries to navigate. The project is intentionally single-purpose and lightweight.

## Key conventions

- Keep the repository minimal and easy to read.
- Prefer straightforward Python without introducing framework or packaging conventions unless the project clearly expands beyond a profile repo.
- Treat `README.md` as profile content, not as app documentation or product guidance.
- Keep changes small and self-contained; there is no existing multi-file architecture to maintain.
- When adding new scripts, place them under `main/` and keep them easy to run directly from the command line.
