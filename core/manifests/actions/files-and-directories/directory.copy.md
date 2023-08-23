---
description: 'Action: directory.copy'
---

# Directory

Creates or copies a given directory into a local location.

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `directory.copy` or `directory.create` |
| `from` | string | no | source file |
| `to` | string | no | destination file |

### Example

```yaml
- action: directory.copy
  from: managed_directory
  to: /root/location
```

