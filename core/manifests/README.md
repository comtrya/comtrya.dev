# Manifests

A manifest in `Comtrya` is a collection of actions and dependencies.

This manifest file can be placed in any location.

Let's assume we have the file `one.yaml`, which looks like this:

```
# one.yaml
actions:
- action: command.run
  command: echo Hello, world!
```

This manifest performs a single task, which uses the `command.run` [action](actions/) and provides the command to be run which is `echo Hello, world!`

Now, let's define `two.yaml` which contains a depdency on `one.yaml`

```
# two.yaml
depends:
- one

actions:
- action: command.run
  command: echo Hello, back!
```



{% content-ref url="actions/" %}
[actions](actions/)
{% endcontent-ref %}

{% content-ref url="depends.md" %}
[depends.md](depends.md)
{% endcontent-ref %}
