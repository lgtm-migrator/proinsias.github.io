---
layout: single
title: "(TIL) Git: Untrack A File Without Deleting It"
date:
modified:
---

Generally when I invoke `git rm <filename>`, I do so with the intention of
removing a file from the project entirely. `git-rm` does exactly that,
removing the file both from the index and from the working tree.

If you want to untrack a file (remove it from the index), but still have it
available locally (in the working tree), then you are going to want to use
the `--cached` flag.

```bash
git rm --cached <filename>
```

If you do this, you may also consider adding that file to the `.gitignore`
file.

Via [jbranchaud/til](https://github.com/jbranchaud/til).