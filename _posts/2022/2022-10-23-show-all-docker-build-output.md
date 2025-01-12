---
modified: '2022-10-23 19:07 -0400'
date: '2022-10-23 19:07 -0400'
layout: single
published: true
title: Show all Docker build output
excerpt: Ensure all layer commands are visible
categories: til
tags:
  - til
  - docker
---
You may have noticed with newer versions of Docker that the output of each layer's commands is shown only while that layer is being built, and is then hidden.

You can control this behavior the `--progress` output of the `docker build` command:

```bash
docker build --help
...
  --progress string         Set type of progress output (auto, plain, tty).
                            Use plain to show container output (default "auto")
```

Via [stackexchange.com](https://devops.stackexchange.com/a/12774).
