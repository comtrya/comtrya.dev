# command.run

| Key | Typ | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | Values: `command.run` |
| `command` | string | no | command to run |
| `args` | string | no | argument passed |
| `dir` | string | no | actual working directory |

## Examples

```yaml
- action: command.run
  command: COMMAND
  args: ["ARGUMENT"]
  dir: .
```

