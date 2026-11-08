# SWE-bench Verified 500: trajectory export by outcome

## Setup

- **Benchmark**: SWE-bench Verified (500 instances)
- **Model**: DeepSeek-V4.1-Flash-1017 (API model name: `deepseek-flash`)
- **Agent**: mini-swe-agent

## Layout

- `success/ids.txt`: resolved instance IDs.
- `success/trajectories/`: original full trajectories for resolved instances.
- `failure/ids.txt`: unresolved and Harness-error instance IDs.
- `failure/trajectories/`: original full trajectories for failures.
- `failure/unresolved_ids.txt`: tests completed but did not resolve.
- `failure/harness_error_ids.txt`: tests not graded successfully (e.g. timeout).
- `index.csv`: per-instance status, source run and trajectory SHA-256.

## Notes

- Files are independent copies, not symbolic links.
- A Harness timeout means the test was not successfully graded. Do not count it as an unresolved instance; it belongs to the Harness-error category. Do not interpret a Harness timeout as a successfully completed unsuccessful test.
