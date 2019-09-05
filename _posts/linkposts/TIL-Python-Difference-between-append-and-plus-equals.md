---
layout: single
title: "(TIL) Python: Difference between append and '+='"
date:
modified:
---

In many applications `+=` and `append` are interchangeable,
but for Python `list`s they are not.

If you are `append`ing a `list` of `list`s to another `list` of `list`s,
`append` will only `append` the first `list`;
you need to use `+=` in order to join all of the `list`s at once.

Via [Kaggle.com](https://www.kaggle.com/c/word2vec-nlp-tutorial/details/part-2-word-vectors).