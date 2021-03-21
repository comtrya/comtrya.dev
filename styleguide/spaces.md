---
description: Add spaces between tasks
---

# Spaces

{% hint style="info" %}
### add spaces between tasks
{% endhint %}

### Good

```yaml
actions:
  - action: package.install
    name: package1_name

  - action: package.install
    name: package2_name
```

### Bad

```yaml
actions:
  - action: package.install
    name: package1_name
  - action: package.install
    name: package2_name
```

