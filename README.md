# asdf-azure-cli ![CI](https://github.com/itspngu/asdf-azure-cli/workflows/CI/badge.svg) ![Lint](https://github.com/itspngu/asdf-azure-cli/workflows/Lint/badge.svg)

[azure-cli](https://github.com/Azure/azure-cli) plugin for the [asdf version manager](https://asdf-vm.com).

## ARCHIVAL NOTICE

I stopped using asdf-vm and archived this repository. If you're using this plugin, please consider forking the repository and having it added to the upstream plugin list at https://github.com/asdf-vm/asdf-plugins.

## Contents

- [Plugin Dependencies](#plugin-dependencies)
- [Install](#install)
- [License](#license)

## Plugin Dependencies

- `curl` - for azure-cli downloads from upstream releases
- `python3` (with `pip` and `venv` modules) - for installing and running the cli

## Install

Plugin:

```shell_session
$ asdf plugin-add azure-cli https://github.com/itspngu/asdf-azure-cli
```

azure-cli:

```shell_session
# Show all installable versions
$ asdf list-all azure-cli

# Install specific version
$ asdf install azure-cli latest

# Set a version globally (in your ~/.tool-versions file)
$ asdf global azure-cli latest

# Run azure-cli
$ az --version
azure-cli                         2.32.0
[...]
```

Refer to the [upstream azure-cli repository](https://github.com/Azure/azure-cli) for documentation and usage instructions.

Check the [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to install & manage versions.

## License

See [LICENSE](LICENSE)
