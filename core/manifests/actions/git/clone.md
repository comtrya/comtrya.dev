---
description: 'Action: git.clone'
---

# Run

| Key          | Typ    | Optional | Description           |
| :----------- | :----- | :------- | :-------------------- |
| `action`     | string | no       | `git.clone`           |
| `repository` | string | no       | repository to clone   |
| `directory`  | string | no       | directory to clone to |

## Example

```yaml
- action: git.clone
  repository: comtrya/comtrya
  directory: {{ user.home_dir }}/Code/src/
```
