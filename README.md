# Limanix community files

[![License: Apache-2.0](https://img.shields.io/github/license/limanix/.github?label=license)](LICENSE)

Shared contribution guidelines, issue templates, and the public profile for the
[Limanix organization](https://github.com/limanix).

| File | Purpose |
| --- | --- |
| [profile/README.md](profile/README.md) | Public organization profile. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution guidelines. |
| [SECURITY.md](SECURITY.md) | Private vulnerability reporting. |
| [.github/ISSUE_TEMPLATE/](.github/ISSUE_TEMPLATE/) | Bug reports, feature requests, and questions. |
| [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) | Change description and verification. |

## Inheritance

GitHub uses these community files when a repository in the organization does
not provide its own file of the same type. A repository's issue templates or
issue-template configuration replace the entire shared issue-template set.

This repository must remain public. Changes take effect after they reach `main`;
the files are not copied into consumer repositories. See
[GitHub's inheritance rules](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

Build instructions, CI workflows, and release configuration belong to each
project. Labels, merge settings, and branch protection are managed in GitHub
settings, not inherited from this repository. Each project also needs its own
license file.
