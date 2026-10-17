# jpe-splunk

jpe-splunk holds its organization profile and describes a focus on log analysis
and event processing.

## Shared CI and releases

- Reuse workflows from `JacobPEvans/.github` and `JacobPEvans/.github-ai`.
  Reference both at `@v1`; never pin them to a commit SHA.
- Keep organization-managed CI and release steps in the reusable workflows.
  Local workflow files should call the shared implementation with repository
  specific inputs.
- Give each repository exactly one `release.yml` caller for its release
  workflow.
- Configure Renovate to extend only `github>JacobPEvans/.github`.
- Enterprise rulesets inject required checks. Do not add repository copies of
  shared checks.

## Repository map

| Repository | Purpose |
| --- | --- |
| `.github` | Organization profile |
