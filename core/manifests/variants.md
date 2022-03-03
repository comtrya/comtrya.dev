# Variants

All Comtrya actions support the concept of variants. Variants allow you to modify how the action will be executed based on the contexts available.

Let's assume you want to run a command that is different on macOS, Linux, and Windows.

```
actions:
  # This action has a "default" execution for when the variants don't overlay,
  # as it does not provide its own "where"
  - action: command.run
    command: echo
    args:
      - hello, world!
    variants:
      - where: os.name == "linux"
        command: reboot
      - where: os.name == "macos"
        command: echo
        args: ["Hello", "macOS"]
      - where: user.username == "rawkode"
        command: echo
        args: ["Hello", "rawkode!"]
```

We even allow you to target the Linux family and specific distribution:

```
actions:
  - action: command.run
    command: echo
    args:
      - hello, vanilla Linux!
    variants:
      - where: os.family == "Debian"
        command: echo Hi, Debian
      - where: os.distribution == "Ubuntu"
        command: echo Hi, Ubuntu
      - where: os.bitness == "64-bit"
        command: echo Hi, 64 bit!
```

Lastly, the `where` clause can be used to selectively skip or run tasks:

```
actions:
  - action: command.run
    where: os.name == "linux"
    command: echo
    args:
      - Hello Linux
```
