---
layout: single
title: "(TIL) Git: Untrack A Directory Of Files Without Deleting"
date:
modified:
---

In [Untrack A File Without Deleting It](untrack-a-file-without-deleting-it.md),
I explained how a specific file can be removed from tracking without
actually deleting the file from the local file system. The same can be done
for a directory of files that you don't want tracked. Just use the `-r`
flag:

```bash
git rm --cached -r <directory>
```

Via [jbranchaud/til](https://github.com/jbranchaud/til).