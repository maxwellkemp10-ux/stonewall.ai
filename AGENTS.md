# Repository Guidelines

## Project Structure & Module Organization
`Stonewall` is a legal document intelligence platform with automation scripts in `scripts/`, test coverage in `tests/`, and CI/CD in `.github/workflows/`. AI agent configurations live in `.claude/` and `agents/`. The platform integrates with Notion for case management and OneDrive for document storage.

## Build, Test, and Development Commands
- `node --test tests/tracker_helpers.test.mjs` runs the Node helper tests.
- `node --test tests/email_consolidator.test.mjs` runs the email consolidator tests.
- `python -m unittest tests.test_ingest_onedrive tests.test_verify_repo_consistency tests.test_tactical_brief` runs the Python test suite.
- `python scripts/repo_sweep.py` performs repo hygiene checks.
- `python scripts/verify_repo_consistency.py` validates catalog and repo alignment.
- `uv run python scripts/ingest_onedrive.py refresh-cases` refreshes the local case cache from Notion.
- `.\scripts\ingest_onedrive.ps1 ingest --root firm --glob "*.pdf" --limit 20` is the PowerShell shortcut for narrow intake runs.

## Coding Style & Naming Conventions
Use 4-space indentation in Python and keep ESM-style JavaScript consistent with existing files in `scripts/`. Prefer descriptive, lowercase-with-underscores Python filenames such as `verify_repo_consistency.py`. All environment-specific values (database IDs, API keys, file paths) must come from environment variables — never hardcode them.

## Testing Guidelines
Add or update tests when changing `scripts/`. Place Python tests in `tests/` using `test_*.py`. Keep Node tests as `.test.mjs` files mirroring the script they cover. Before opening a PR, run the targeted suite for the surface you changed.

## Commit & Pull Request Guidelines
Use short, imperative commit subjects. Keep each commit scoped to one logical change. PRs should state what changed, which surfaces were touched (`scripts/`, `tests/`, `.github/`), and any required follow-up in Notion or OneDrive.

## Environment & Configuration
All sensitive values are loaded from environment variables. Copy `.env.example` to `.env` and populate before running any scripts. Required variables are documented in `.env.example`. Never commit `.env` or any file containing API keys, tokens, or database IDs.

## Security & Configuration Tips
Do not commit real Notion database IDs, personal file paths, or API keys. Use placeholder values in examples (e.g., `YOUR_NOTION_DATABASE_ID`). `refresh-cases` and `sync-notion` require `NOTION_TOKEN`. Read `CLAUDE.md` before major repo work.
