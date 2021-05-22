---
description: Getting Started with the CLI
---

# CLI

```bash
comtrya <manifest-location> [FLAGS] [OPTIONS]
```

`comtrya <manifest-location> [FLAGS] [OPTIONS]`

 **Comtrya supports local and remote manifest locations. See examples below**

## Flags

* `comtrya -h, --help` Prints help information
* `comtrya -V, --version` Prints help information
* `comtrya -v, --verbose` Debug & tracing mode \(-v, -vv\)

## Options

* `comtrya -m, --manifests <manifests>...` Run a subset of your manifests, comma separated list

## ARGS

* `comtrya <manifest-location>` Manifests can come from multiple locations, such as local directory or Git repository.

## Examples

```bash
# Manifests in a local directory
comtrya .

# Manifests in a Git repository
comtrya https://github.com/rawkode/rawkode

# Execute a single manifest from a local directory
comtrya . -m EXAMPLE

# Execute multiple manifests from a local directory
comtrya . -m EXAMPLE,TEST
```

