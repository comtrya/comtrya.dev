# Real world

#### Install a package and execute a shell script

```yaml
actions:
  - action: package.install
    name: package_name
    repository: homebrew/cask

  - action: command.run
    command: bash
    args: ["-c", "./package_name/files/install.sh"]
    dir: .
```

#### Install a package and copy the configuration file

```yaml
actions:
  - action: package.install
    name: package_name

  - action: file.copy
    from: package_name_config
    to: "{{ user.home_dir }}/.package_name_config"
    chmod: 644
```

#### Install a package and copy the configuration directory

```yaml
actions:
  - action: package.install
    name: package_name
    repository: homebrew/cask
  
  - action: directory.copy
    from: SOURCE_DIR
    to: "{{ user.home_dir }}/.package_name"
```

