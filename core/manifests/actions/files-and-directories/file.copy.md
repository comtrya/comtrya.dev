---
description: 'Action: file.copy'
---

# File

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `file.copy` |
| `from` | string | no | source file |
| `to` | string | no | destination file |
| `template` | bool | yes | renderes files using [context providers](../../../contexts-1/context-provider.md), Default: `false` |
| `chmod` | int | yes | octal permissions |

### Example

```yaml
- action: file.copy
  from: managed_file
  to: /root/file
  template: true
  chmod: 644
```

