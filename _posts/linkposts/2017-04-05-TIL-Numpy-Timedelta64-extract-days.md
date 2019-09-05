---
layout: single
title: "(TIL) Numpy: Extract days from timedelta64"
date: 2017-04-05 21:31
modified: 2017-04-05 21:31
---

To extract the integer value of days from a `numpy.timedelta64`, you divide it with a
`timedelta64` of one day:

```python
>>> x = np.timedelta64(2069211000000000, 'ns')
>>> days = x.astype('timedelta64[D]')
>>> days / np.timedelta64(1, 'D')
23
```

Via [StackOverflow](https://stackoverflow.com/questions/18215317/extracting-days-from-a-numpy-timedelta64-value).