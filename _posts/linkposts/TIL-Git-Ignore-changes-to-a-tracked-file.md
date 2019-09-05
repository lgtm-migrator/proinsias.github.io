---
layout: single
title: "(TIL) Git: Ignore Changes To A Tracked File"
date:
modified:
---

Files that should never be tracked are listed in your `.gitignore` file. But
what about if you want to ignore some local changes to a tracked file?

You can tell git to assume the file is unchanged

```bash
git update-index --assume-unchanged <some-file>
```

Reversing the process can be done with the `--no-assume-unchanged` flag.

Via [jbranchaud/til](https://github.com/jbranchaud/til).