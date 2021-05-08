# Command.run

#### 

```yaml
# Example 1 - execute a command   
- action: command.run
  command: echo
  args: ["hi"]
  dir: .
  
# Example 2 - execute a script
- action: command.run
  command: bash
  args: ["-c", "./package_name/files/install.sh"]
  dir: .
```

