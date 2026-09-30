# Contributing

Open an issue or pull request in the repository affected by your change.
Search existing issues and pull requests before opening a new one.

Please follow the [Code of Conduct](https://github.com/limanix/.github/blob/main/CODE_OF_CONDUCT.md).

## Issues

- **Bug report:** use the issue form. Include the affected version or commit and a minimal reproduction when possible. Remove credentials and private data from logs and configuration files.
- **Feature request:** describe the problem, use case, and limitation first. A configuration or command example is optional.
- **Documentation:** use the Documentation issue form for missing, unclear, or outdated content.
- **Question:** use the question form.

Report vulnerabilities privately using the [security policy](https://github.com/limanix/.github/blob/main/SECURITY.md).

## Pull requests

1. For anything beyond a small fix, open an issue first and agree on the approach before coding.
2. Keep a PR focused on one change. With squash merge, the PR title becomes the commit title. Release notes use PR titles; write one that reads well in a changelog.
3. Run the checks described in the target repository's README or development guide, and review its CI results where workflows are configured.
4. Every PR needs **at least one release label** (`feature`, `bug`, `docs`, `deps`, `tooling`, `other`, or `skip`). External contributors do not need label permissions: if you cannot add the label, a maintainer adds it during review. The `check label` job stays red until then.

## Dev loop

The `client`, `modules`, and `docs` repositories use a [Taskfile](https://taskfile.dev) ([installation](https://taskfile.dev/installation/)).
From the target repository directory, list its available tasks:

```bash
task -l
```

Follow that repository's README or development guide for the relevant `ci/*` tasks and prerequisites.
Some tasks run in Docker; native client builds require macOS and the Xcode command-line tools.

## Releases

The [release process](https://limanix.dev/releases/index.html) documents how merged pull requests become client, modules, and documentation releases.
For published versions and release notes, see the target repository's GitHub Releases page.
The client and modules release workflows generate release notes from merged pull requests.

## License

LimaNix projects are licensed under Apache-2.0.
By contributing, you agree that your contribution is licensed under the same terms.
