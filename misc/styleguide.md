# Styleguide

## Use yaml instead of yml

> Pease use ".yaml" when possible - [YAML.org](https://yaml.org/faq.html)

```bash
# Good
manifest.yaml

# Bad
manifest.yml
```

## Use the correct order of keywords

```yaml
# Good
actions:

depends:

# Bad
depends:

actions:

```

## Add spaces between tasks

```yaml
# Good
actions:
  - action: package.install
    name: package1_name

  - action: package.install
    name: package2_name
    
# Bad
actions:
  - action: package.install
    name: package1_name
  - action: package.install
    name: package2_name

```

## Use 2 spaces for indentation

```yaml
# Good
actions:
  - name: firefox-developer-edition
    action: package.install
    variant:
      ubuntu:
        name: firefox
        repository: ppa:mozillateam/firefox-next
        
# Bad
actions:
    - name: firefox-developer-edition
        action: package.install
        variant:
              ubuntu:
                    name: firefox
                    repository: ppa:mozillateam/firefox-next

```

## Wrap variables in spaces

```yaml
# Good
actions:
  - action: file.copy
    from: default.yaml
    to: "{{ user.home_dir }}/default.yaml"
    
# Bad
actions:
  - action: file.copy
    from: default.yaml
    to: "{{user.home_dir}}/default.yaml"

```

