# composerx

The same that `pipx` is for `pip`, `composerx` is for `composer`.

It allows you to install and run global PHP CLI tools in isolated environments.

## Why?

```bash
composer global require laravel/installer
```

It will install the `laravel/installer` package in special global composer directory in `~/.config/composer` and it can potentially conflict with other global packages.

With `composerx`, each global package is installed in its own directory in `~/.local/share/composerx/{PACKAGE_NAME}`, avoiding dependency conflicts and symlink to the binary is created in `~/.local/bin`.

## Commands

| Command   |
| --------- |
| install   |
| uninstall |
| list      |
| run       |

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.