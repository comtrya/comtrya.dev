---
description: 'Action: package.install'
---

# Install

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `package.install` |
| `name` | string | no | name of the target package |
| `list` | list | yes | list of multiple packages |
| `provider` | string | yes | OS specific package provider |
| `repository` | string | yes | specific repository for a provider & package |

### Example

{% tabs %}
{% tab title="Basic" %}
```yaml
- action: package.install
  name: curl
```
{% endtab %}

{% tab title="List" %}
```yaml
- action: package.install
  list:
  - curl
  - wget
```
{% endtab %}

{% tab title="Providers" %}
```yaml
- action: package.install
  name: curl
  provider: homebrew
  # Providers are guessed when missing, valid options are:
  # aptitude, bsdpkg, homebrew, winget, and yay/pacman
```
{% endtab %}

{% tab title="Repositories" %}
```yaml
# When specifying a provider, you can attempt to provide
# repository information: like ppa's or taps

- action: package.install
  name: blox
  provider: homebrew
  repository: cueblox/tap
```
{% endtab %}

{% tab title="Variants \(Alpha\)" %}
```yaml
# Very early preview feature
- action: package.install
  name: kubectl
  variants:
    macOS:
      name: kubernetes-cli
  
```
{% endtab %}

{% tab title="Jinja \(Discouraged\)" %}
```
# We want to provide better declarative options than this, but it works
# if needed.

{% if user.username == "root" %}
- action: package.install
  name: kubectl
{% endif %}
```
{% endtab %}
{% endtabs %}

