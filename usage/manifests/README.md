# Manifests

A manifest in `Comtrya` is a collection of actions and dependencies.

```text
# one.yaml
actions:
- action: command.run
  command: echo Hello, world!

# two.yaml
depends:
- one

actions:
- action: command.run
  command: echo Hello, back!
```

{% page-ref page="actions/" %}

{% page-ref page="depends.md" %}

