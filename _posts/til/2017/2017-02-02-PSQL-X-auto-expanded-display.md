---
layout: single
title: "(TIL) PSQL: Auto Expanded Display"
date: 2017-02-02 20:57
modified: 2017-02-02 20:57
categories: til
tags:
  - psql
  - sql
  - til
---

By default, postgres has expanded display turned off. This means that
results of a query are displayed *horizontally*.
At times, the results of a query can be so wide that line wrapping occurs.
This can make the results and their corresponding column names rather
difficult to read. In these situations, it is preferable to turn on expanded
display so that results are displayed *vertically*.
The `\x` command can be used to toggle expanded display on and off.

Having to toggle expanded display on and off depending on the way a
particular set of results is going to display can be a bit tedious.
Fortunately, running `\x auto` will turn on auto expanded display. This
means postgres will display the results normally when they fit and only
switch to expanded display when it is necessary.

Via [jbranchaud/til](https://github.com/jbranchaud/til).