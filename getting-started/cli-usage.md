---
description: Getting Started with the CLI
---

# CLI

```bash
comtrya apply
comtrya apply -d <manifest-location>
comtrya apply -m <comma,separated,manifest,names>
comtrya apply -l <label-name>
```

{% hint style="info" %}
&#x20;Comtrya supports local and remote manifest locations. See examples below
{% endhint %}

## Flags

* `comtrya -h, --help` Prints help information
* `comtrya -V, --version` Prints help information
* `comtrya -v, --verbose` Debug & tracing mode (-v, -vv)

## Examples

```bash
# Manifests in a local directory
comtrya apply

# Manifests in a Git repository
comtrya -d https://github.com/rawkode/rawkode apply

# Manifests in a Git repository with a branch and path
comtrya -d https://github.com/rawkode/rawkode#main:dotfiles apply

# Manifests in a Git repository with a branch and path and a subset selector
comtrya -d https://github.com/rawkode/rawkode#main:dotfiles apply -m dev.git

# Execute a single manifest from a local directory
comtrya apply -m manifest-name

# Execute multiple manifests from a local directory
comtrya apply -m manifest-1,manifest-2
```
