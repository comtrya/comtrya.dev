---
description: 'Action: user.add'
---

# Add user

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | Values: `user.add` |
| `username` | string | no | Username of the new user to add |
| `home_dir` | string | yes | Specifies the home directory of the user to create |
| `fullname` | string | yes | The full name of the user being added  |
| `shell` | string | yes | For UNIX systems, specify the shell for the user |
| `provider` | string | yes | OS specific package provider |

### Example

```yaml
actions:
  - action: user.add
    username: test
    shell: sh
    home_dir: /home/test
```

