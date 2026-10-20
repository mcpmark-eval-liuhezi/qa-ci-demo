# qa-ci-demo

Live setup for the QA onboarding workshop module: **debugging a failed CI run end to end**.

## What's here

| Item | Location |
|---|---|
| Workflow `demo-fail` | [`.github/workflows/demo-fail.yml`](.github/workflows/demo-fail.yml) |
| Failed run (#1, conclusion: failure) | https://github.com/mcpmark-eval-liuhezi/qa-ci-demo/actions/runs/39369135433 |
| Failed job `build` (ID 118452769018) | https://github.com/mcpmark-eval-liuhezi/qa-ci-demo/actions/runs/39369135433/job/118452769018 |
| Archived log of the failed job (permanent reference) | [`evidence/demo-fail-build-job.log`](evidence/demo-fail-build-job.log) |
| Raw log (for download) | https://raw.githubusercontent.com/mcpmark-eval-liuhezi/qa-ci-demo/main/evidence/demo-fail-build-job.log |

## The failure

The workflow prints a build correlation ID and then intentionally exits with code 3:

- Correlation ID: `BUILD-CORRELATION-ID QA-CI-8F3K2`
- Failing step: `fail` → `##[error]Process completed with exit code 3.`

## Workshop exercise

1. Open the failed run and locate the failing job and step.
2. Pull the job log and find the correlation ID line and the exit code.
3. Download `evidence/demo-fail-build-job.log` (or the raw URL above) and upload it through the practice file upload form to attach your evidence.
