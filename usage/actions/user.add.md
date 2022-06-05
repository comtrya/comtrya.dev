# user.add

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | Values: `user.add` |
| `username` | string | no | Username of the new user to add |
| `home_dir` | string | yes | Specifies the home directory of the user to create |
| `fullname` | string | yes | The full name of the user being added  |
| `shell` | string | yes | For UNIX systems, specify the shell for the user |
| `provider` | string | yes | OS specific package provider |

## Passwords

Currently the implementation is left up to the individual provider. On UNIX and UNIX-like systems, the default implementation will be to generate a random password for the user.

## Examples

```yaml
actions:
  - action: user.add
	username: test
	fullname: Test User
	shell: sh
	home_dir: /home/test
```
