# Indentation

{% hint style="info" %}
### use 2 spaces for indentation
{% endhint %}

### Good

```yaml
actions:
  - name: firefox-developer-edition
    action: package.install
    variant:
      ubuntu:
        name: firefox
        repository: ppa:mozillateam/firefox-next
```

### Bad

```yaml
actions:
    - name: firefox-developer-edition
        action: package.install
        variant:
              ubuntu:
                    name: firefox
                    repository: ppa:mozillateam/firefox-next
```

