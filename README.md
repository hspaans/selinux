# SELinux Modules

Modules for SELinux

## Modules

| Module | State | Note                                        |
| :----: | :---: | ------------------------------------------- |
| vscode | Alpha | Using VSCode Devcontainers with Moby-Engine |

## Installing a module

```shell
checkmodule -M -m -o module.mod modules.te
semodule_package -o module.pp -m module.mod
sudo semodule -i module.pp
```

## Uninstalling a module

```shell
sudo semodule -u module.pp
```
