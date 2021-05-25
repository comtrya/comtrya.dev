# Symlinks

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `file.link` |
| `from` | string | no | symlink location |
| `to` | string | no | symlink points to |

### Example

```yaml
- action: file.link
  from: /root/symlink
  to: managed_file
```

