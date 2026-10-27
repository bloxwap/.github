# .github

Shared reusable workflows for bloxwap repositories.

## v1.1.0

- New opt-in `semgrep` job (`semgrep: true`, `semgrep-config` default `p/default`). Report-only: `continue-on-error`, always exits 0, and is not a `gate` dependency, so it never fails or gates a run.
- Semgrep 1.182.1 runs through uv 0.13.6 (SHA-256 verified, cached in the runner tool cache) with `--metrics=off`. The job summary lists counts and up to 100 High/Medium findings (rule, path, line; no source excerpts). Slack is posted only when High (`ERROR`) findings exist, `notify-slack` is on, and the event is not a pull request.
- `gate` now runs only when one of deps, secrets, iac or workflow-lint is enabled, so a Semgrep-only weekly caller does not fail on an empty gate. Defaults and all v1.0.x inputs are unchanged.

## v1.0.2

- Tool downloads retry all curl errors and use up to four attempts with exponential backoff (5, 15, 45 seconds). Each curl invocation retries five times, with a 20-second connection timeout and a 180-second transfer timeout; existing job timeouts still apply.
- SHA-256 verification precedes atomic cache writes. Verified warm caches retain their existing paths; invalid cached packages are removed and downloaded again. URL and checksum pins are unchanged.
- Nightly workflow lint warns and skips linting if tool downloads fail in report-only mode. With `enforce-workflow-lint: true`, installation failures fail the job. Scanner downloads in both reusable workflows remain fail-closed.
