---
description: Getting Started with the CLI
---

# CLI

```bash
comtrya <manifest-location> [FLAGS] [OPTIONS]
```

{% hint style="info" %}
&#x20;Comtrya supports local and remote manifest locations. See examples below
{% endhint %}

## Flags

* `comtrya -h, --help` Prints help information
* `comtrya -V, --version` Prints help information
* `comtrya -v, --verbose` Debug & tracing mode (-v, -vv)

## Options

* `comtrya -m, --manifests <manifests>...` Run a subset of your manifests, comma separated list

## Arguments

* `comtrya <manifest-location>` Manifests can come from multiple locations, such as local directory or Git repository.

## Examples

```bash
# Manifests in a local directory
comtrya .

# Manifests in a Git repository
comtrya https://github.com/rawkode/rawkode

# Manifests in a Git repository with a branch and path
comtrya https://github.com/rawkode/rawkode#main:dotfiles

# Execute a single manifest from a local directory
comtrya . -m EXAMPLE

# Execute multiple manifests from a local directory
comtrya . -m EXAMPLE,TEST
```

{% hint style="info" %}
We plan on supporting the same Git "syntax" that `docker image build` [supports](https://docs.docker.com/engine/reference/commandline/build/#git-repositories) for remote build contexts. You can [subscribe to progress here](https://github.com/comtrya/comtrya/issues/107).

Missing ones are:



```
myrepo.git#pull/42/head
```
{% endhint %}
