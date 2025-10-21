# openSourceContributions
You can fine all my open-source contributions here!

Contribution #1: For: https://github.com/TEAMMATES/teammates
- Issue # 13356
- Outline of Solution
- This PR updates the GitHub Actions workflow files to prevent expensive E2E and accessibility tests from running on every commit.
- Changed axe.yml, e2e.yml, and e2e-sql.yml to be triggered manually via workflow_dispatch: instead of on push and pull_request.
- The schedule: for the E2E tests is kept, so they will still run daily.
- This resolves the issue where developers had to run a full test suite for minor changes or when merging master.
- pull request: https://github.com/TEAMMATES/teammates/pull/13380

