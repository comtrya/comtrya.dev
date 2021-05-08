# File.copy

#### 1

```yaml
actions:
  - action: file.copy
    from: config
    to: "{{ user.home_dir }}/.config/git/config"
    template: true
    chmod: 644
```

