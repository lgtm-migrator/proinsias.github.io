---
layout: single
title: "(TIL) Nix: Save matching and non matching lines with awk"
date:
modified:
---

```bash
awk '/pattern/ {print $0 >"yes.csv"; next}{print $0 >"no.csv"}' input.csv
```