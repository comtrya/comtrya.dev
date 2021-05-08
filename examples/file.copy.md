# File.copy

#### Copy a source file to a destination file

```yaml
- action: file.copy
  from: package_name_config
  to: "{{ user.home_dir }}/.package_name_config"
  chmod: 644
```



