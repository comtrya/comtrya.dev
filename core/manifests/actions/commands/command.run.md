---
description: 'Action: command.run'
---

# Run

| Key | Typ | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `command.run` |
| `command` | string | no | command to run |
| `args` | string | no | argument passed |
| `dir` | string | no | actual working directory |

## Example

```yaml
- action: command.run
  dir: .
  command: echo
  args:
  - Hello world
```



