---
layout: single
title: 'Git: Sort branches by recency'
excerpt: A more useful default behavior
date: 2021-04-27 20:49
modified: 2021-11-02 20:49
categories: til
tags:
    - git
    - til
---

> When you type git branch, your branch list is sorted alphabetically by default.
> This isn't super helpful. To sort your branches by their last commit date,
> with the most recent at the top, add this to your `.gitconfig`:

```git
[branch]
  sort = -committerdate
```

Via [Adam Hollett](https://dev.to/admhlt/terminal-tricks-from-my-dotfiles-2moe).
