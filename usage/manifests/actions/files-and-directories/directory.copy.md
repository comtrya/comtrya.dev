# Directory

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `directory.copy` |
| `from` | string | no | source file |
| `to` | string | no | destination file |

### Example

```yaml
- action: directory.copy
  from: managed_directory
  to: /root/location
```

