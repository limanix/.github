# Contributing

Open an issue or pull request in the repository affected by your change.
Search existing issues and pull requests before opening a new one.

## Issues

For bugs, include the version or commit, a minimal reproduction, expected and
actual behavior, and relevant logs. Remove credentials and private data from
logs and configuration files.

For feature requests, describe the use case and the limitation you encountered.
Discuss changes to public interfaces or behavior before starting a large rewrite.

Report vulnerabilities privately using the
[security policy](https://github.com/limanix/.github/blob/main/SECURITY.md).

## Pull requests

Keep each pull request focused on one change. Use a title that describes the
result, explain why the change is needed, and link related issues.

Follow the target project's README and development documentation for setup and
checks. Use its existing `ci/*` tasks when available. Describe the checks you ran
and anything left unverified; include manual verification for affected VM or
module behavior. Update examples and documentation when usage changes.

Maintainers apply the relevant release-note labels: `bug`, `feature`, `deps`,
`docs`, `tooling`, `other`, or `skip`. These labels classify the pull request;
contributors do not need label permissions to submit one.
