# Variables

{% hint style="info" %}
### wrap vars in spaces
{% endhint %}

### Good

```yaml
actions:
  - action: file.copy
    from: default.yaml
    to: "{{ user.home_dir }}/default.yaml"
    template: false
```

### Bad

```yaml
actions:
  - action: file.copy
    from: default.yaml
    to: "{{user.home_dir}}/default.yaml"
    template: false
```

