---
layout: single
title: "(TIL) Tmux: Pane Killer"
date:
modified:
---

The current pane can be _killed_ (closed) using the following key binding:

```tmux
<prefix>x
```

You will be prompted to confirm with either `y` or `n`.

If there is only one pane in the current window, then the window will be
_killed_ along with the pane.

Via [jbranchaud/til](https://github.com/jbranchaud/til).