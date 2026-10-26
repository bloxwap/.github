# .github

Shared reusable workflows for bloxwap repositories.

## v1.0.2

- Tool downloads retry all curl errors and use up to four attempts with exponential backoff (5, 15, 45 seconds). Each curl invocation retries five times, with a 20-second connection timeout and a 180-second transfer timeout; existing job timeouts still apply.
- SHA-256 verification precedes atomic cache writes. Verified warm caches retain their existing paths; invalid cached packages are removed and downloaded again. URL and checksum pins are unchanged.
- Nightly workflow lint warns and skips linting if tool downloads fail in report-only mode. With `enforce-workflow-lint: true`, installation failures fail the job. Scanner downloads in both reusable workflows remain fail-closed.
