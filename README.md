---
description: Configuration Management for Localhost
---

# Comtrya

### Comtrya

![Harlan from SG-1 saying &quot;Comtrya!&quot;](.gitbook/assets/comtrya.gif)

Comtrya is a tool that allows you to configure and provision an operating system through YAML based manifests. Comtrya's goals are:

1. Run on any operating system
2. Provide a simple YAML interface to, potentially, complex tasks

### Comparison to Alternatives

#### Ansible

Ansible is a great tool task runner, but comes with a lot of modules that aren't really necessary for localhost provisioning and can be cumbersome to run individual tasks within a playbook.

#### SaltStack

SaltStack has been a favourite of mine \(@rawkode\) for many years, and while it's event system is a game changer for working with many devices - it's inability to display progress of large state runs makes it cumbersome to use for localhost provisioning.



