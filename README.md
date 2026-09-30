# LimaNix community files

[![License: Apache-2.0](https://img.shields.io/github/license/limanix/.github?label=license)](LICENSE)

Shared defaults for [LimaNix](https://github.com/limanix) repositories. They cover contribution guidelines, issue and pull request templates, security and conduct policies, and the organization profile.

This repository has no build or CI. Changes take effect when they reach `main`.

## Contents

| Path                                                                 | Where GitHub shows it                                                      |
|----------------------------------------------------------------------|----------------------------------------------------------------------------|
| [profile/README.md](profile/README.md)                               | The organization page at [github.com/limanix](https://github.com/limanix). |
| [CONTRIBUTING.md](CONTRIBUTING.md)                                   | Linked when someone opens an issue or pull request.                        |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)                             | Linked from the contribution guide and the organization profile.           |
| [SECURITY.md](SECURITY.md)                                           | The **Security** tab of each repository.                                   |
| [.github/ISSUE_TEMPLATE/](.github/ISSUE_TEMPLATE/)                   | Bug, feature, documentation, and question forms on **New issue**.          |
| [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) | The prefilled description of a new pull request.                           |
| [assets/logo/](assets/logo/)                                         | Not shown by GitHub; the organization logo source.                         |

## Inheritance

- GitHub uses a file from this repository when the target repository has no file of the same type in its `.github/` folder, root, or `docs/` folder.
- Issue templates are all-or-nothing. If a repository has valid templates or a `config.yml` in its own `.github/ISSUE_TEMPLATE/`, none of the shared forms are used there.
- Files are not copied. They do not appear in the file tree, history, or clones of the other repositories.
- This repository must stay public.

See [GitHub's rules for default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

## What each repository keeps

Each project keeps these files and settings:

| Item                                      | Location                           |
|-------------------------------------------|------------------------------------|
| License                                   | `LICENSE`                          |
| CI and release workflows                  | `.github/workflows/`               |
| Release label check                       | `.github/workflows/labels.yml`     |
| Release notes categories                  | `.github/release.yml`              |
| Labels, merge settings, branch protection | Repository settings                |
| Private vulnerability reporting           | Repository settings → **Security** |

Issue types used by the shared forms (`Bug`, `Feature`, `Documentation`, and `Question`) are defined once in the organization settings. `Task` is also available for project-specific work.

## Keeping repositories in sync

These documents describe rules that each repository enforces on its own.
When a rule changes, update every place that depends on it.

**Release labels** (`feature`, `bug`, `docs`, `deps`, `tooling`, `other`, `skip`):

1. The labels in every repository, including this one.
2. The label check in each repository's `.github/workflows/labels.yml`.
3. The categories in each repository's `.github/release.yml`.
4. The lists in [CONTRIBUTING.md](CONTRIBUTING.md) and the [pull request template](.github/PULL_REQUEST_TEMPLATE.md).

**Issue forms:**

- Every form assigns an organization issue type by name. Keep the names in the YAML files aligned with the organization settings.
- The forms are inherited by repositories without their own issue-template directory. A repository with local forms must update them separately.

**Merging and releases:** every repository uses squash merge with the pull request title as the commit title.
Release notes use those titles. [CONTRIBUTING.md](CONTRIBUTING.md) asks for titles that read well in a changelog.

**Security:** keep private vulnerability reporting enabled in every repository. [SECURITY.md](SECURITY.md) directs reporters there.

## Making changes

Open a pull request against `main`.
Before merging, open the files on GitHub from your branch to check issue forms and Markdown rendering.
After merging, confirm the result:

- Profile: [github.com/limanix](https://github.com/limanix).
- Forms: **New issue** in a repository without its own templates, for example, [client](https://github.com/limanix/client/issues/new/choose).
- Pull request template: open a draft pull request in any repository.
