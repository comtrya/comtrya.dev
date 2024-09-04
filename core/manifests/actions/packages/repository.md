# Repository

To install a third-party repository (Tap for homebrew for example), Comtrya can interpret this action.

| Key | Type | Optional | Description |
| :--- | :--- | :--- | :--- |
| `action` | string | no | `package.repository` |
| `name` | string | no | name of the target package |
| `repository` | string | yes | specific repository for a provider & package |

### Example

```yaml
- action: package.repository
  provider: homebrew
  name: homebrew/cask-fonts
```
