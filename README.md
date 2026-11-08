# SWE-bench Verified 500: trajectory export by outcome

- `success/ids.txt`: resolved instance IDs.
- `success/trajectories/`: original full trajectories for resolved instances.
- `failure/ids.txt`: unresolved and Harness-error instance IDs.
- `failure/trajectories/`: original full trajectories for failures.
- `failure/unresolved_ids.txt`: tests completed but did not resolve.
- `failure/harness_error_ids.txt`: tests not graded successfully (e.g. timeout).
- `index.csv`: per-instance status, source run and trajectory SHA-256.

Files are independent copies, not symbolic links. Do not interpret a Harness timeout as a successfully completed unsuccessful test.
