# command.run

command.run

| Key | Typ | Optional | Description |
| :--- | :--- | :--- | :--- |
| action | string | no | Values: `command.run` |
| command | string | no |  |
| args | string | no |  |
| dir | string | no |  |

## Examples

```yaml
- action: command.run
  command: echo
  args: ["hi"]
  dir: .
```

