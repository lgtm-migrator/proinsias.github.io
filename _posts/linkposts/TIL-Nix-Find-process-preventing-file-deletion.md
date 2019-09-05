---
layout: single
title: "(TIL) Nix: Find process preventing file deletion with fuser"
date:
modified:
---

Sometimes when deleting a file, the error "File is already in use" is encountered,
with further trouble locating the process using the file.

To find any processes using the file you can use `fuser` command :

```bash
fuser -k filename
```

The command above will search for the file and kill whatever processes are using
it.

Via [enki.com](https://insights.enki.com/insight/55e8d159cc63eb3a0074d1db).