# package.install

#### Basic install

```yaml
actions:
  - action: package.install
    name: package_name
```

#### Install from a specific package provider

```yaml
actions:
  - action: package.install
    name: package_name
    provider: brew
    repository: EXAMPLE/tap
```

#### Install multiple packages

```yaml
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
      - package_name_3
      - ...
```

#### Install multiple packages from a specific package provider

```yaml
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
      - package_name_3
      - ...
    provider: brew
    repository: EXAMPLE/tap
```

