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

{% hint style="warning" %}This feature will no longer be available in main or versions after 0.8.8.{% endhint %}

