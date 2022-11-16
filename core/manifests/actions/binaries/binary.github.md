---
description: 'Action: binary.github'
---

# Run

| Key          | Typ    | Optional | Description                           |
| :----------- | :----- | :------- | :------------------------------------ |
| `action`     | string | no       | `binary.github`                       |
| `name`       | string | no       | name of binary locally after download |
| `directory`  | string | no       | directory to save the binary locally  |
| `repository` | string | no       | GitHub repository                     |
| `version`    | string | no       | version/tag name                      |

## Example

```yaml
- action: binary.github
  name: comtrya
  directory: /usr/local/bin
  repository: comtrya/comtrya
  version: v0.8.0
```
