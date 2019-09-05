---
layout: single
title: "(TIL) Nix: Create A File Descriptor with Process Substitution"
date:
modified:
---

Process substitution can be used to create a file descriptor from the
evaluation of a shell command. The syntax for process substitution is
`<(LIST)` where `LIST` is one or more bash commands.

```bash
$ cat <(echo 'hello, world')
hello, world
```

This is particularly useful for commands that expect files, such as diff:

```bash
$ diff <(echo 'hello, world') <(echo 'hello, mars')
1c1
< hello, world
---
> hello, mars
```

Via [jbranchaud/til](https://github.com/jbranchaud/til).