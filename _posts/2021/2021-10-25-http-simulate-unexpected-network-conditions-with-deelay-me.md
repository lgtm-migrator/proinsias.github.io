---
layout: single
title: "HTTP: Simulate unexpected network conditions with deelay.me"
date: 2021-10-25 13:23
modified: 2021-10-25 13:23
categories: tips
tags:
  - http
  - tips
  - utility
---

> Slow loading resources (images, scripts, etc) can break your application.
> With [this proxy](http://deelay.me) you can simulate unexpected network conditions when loading a specific resource.

To use `deelay.me`, change your link to: https://deelay.me/<delay in
milliseconds>/<original url>. For example:

<https://deelay.me/5000/https://picsum.photos/200/300>