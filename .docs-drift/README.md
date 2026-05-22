# `.docs-drift/`

State and configuration for the **Docs Drift Watcher** — the daily
schedule that keeps the documentation honest about what the code does.

| File | Owner | Purpose |
| --- | --- | --- |
| `config.yml` | Humans | Globs, ignore lists, thresholds. |
| `state.json` | The watcher | Last-run checkpoint. Bumped only when the watcher's PR is merged. |
| `last-run.json` | The watcher | Per-run summary; uploaded as a CI artifact. |

When repository policy blocks Actions from opening PRs with
`GITHUB_TOKEN`, the workflow still pushes the `docs-drift/auto` branch and
finishes green with manual next steps in the job summary. Add
`DOCS_DRIFT_TOKEN` with contents write and pull requests write access to
keep PR open/refresh fully automatic.

The full design and operating notes live at
[`docs/overview/docs-drift-watcher.md`](../docs/overview/docs-drift-watcher.md).
