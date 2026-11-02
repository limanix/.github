<div align="center">
<img src="https://raw.githubusercontent.com/limanix/.github/main/.github/assets/banner/limanix-header.png" alt="LimaNix" width="100%">

<p align="center">
<a href="https://docs.limanix.dev/quick-start"><code>→ Get started</code></a>
<a href="https://docs.limanix.dev/"><code>Documentation</code></a>
<a href="https://docs.limanix.dev/contributing"><code>Contributing</code></a>
</p>

<p align="center"><sub>macOS 26 or newer | Apple Silicon and Intel</sub></p>
</div>

______________________________________________________________________

LimaNix runs Linux development machines on your Mac. You describe a virtual
machine in one file, `limanix.toml`, and the `limanix` command creates it: a
NixOS system with your shell, languages, services and packages. You don't need
to know Nix, and you don't install Lima or Nix on the Mac.

- **One file declares the machine.** It lives beside your project and lists the
  resources, shared folders, shell, toolchains, modules and packages.
- **Your files stay on the Mac.** Project folders and your VM home live on the
  Mac and survive updates, and your editor opens the project in the VM over SSH.
- **Updates build before the VM restarts.** When a build fails, the VM keeps the
  system it had.
- **Modules fit together.** Shell components, toolchains and services share one
  theme, and each toolchain connects its language server to the editor.

## Try it

[Install the client](https://docs.limanix.dev/install), then on your Mac:

```console
limanix first-config
limanix create --config limanix.toml
limanix shell example-box
```

The [quick start](https://docs.limanix.dev/quick-start) goes from the download
to a shell in the VM, then through a change and cleanup.

## Repositories

| Repository | Holds |
| -- | -- |
| [client](https://github.com/limanix/client) | `limanix`, the command on the Mac, with Lima and the catalog inside |
| [lmx](https://github.com/limanix/lmx) | `lmx` and its daemon `lmxd`, inside every VM |
| [modules](https://github.com/limanix/modules) | The [catalog](https://docs.limanix.dev/modules/) of shells, toolchains and services, its themes and prompts, and the base disk |
| [site](https://github.com/limanix/site) | [limanix.dev](https://limanix.dev) and [docs.limanix.dev](https://docs.limanix.dev) |

## Get involved

- Open an issue in the repository it concerns, for questions, bug reports and
  ideas.
- Read the
  [contribution guide](https://github.com/limanix/.github/blob/main/CONTRIBUTING.md)
  before a pull request.
- Report vulnerabilities privately through the
  [security policy](https://github.com/limanix/.github/blob/main/SECURITY.md).
- Follow the
  [Code of Conduct](https://github.com/limanix/.github/blob/main/CODE_OF_CONDUCT.md).

LimaNix is free and open source under the Apache License 2.0.
