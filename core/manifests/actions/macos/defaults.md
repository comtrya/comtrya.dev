---
description: 'Action: macos.default'
---

# Run

| Key      | Typ    | Optional | Description                                              |
| :------- | :----- | :------- | :------------------------------------------------------- |
| `domain` | string | no       | Domain: `defaults domains` or https://macos-defaults.com |
| `key`    | string | no       | Which key to change                                      |
| `kind`   | string | no       | Value type                                               |
| `value`  | string | no       | Value                                                    |

## Example

```yaml
- action: macos.default
  domain: com.apple.dock
  key: orientation
  kind: string
  value: left
```
