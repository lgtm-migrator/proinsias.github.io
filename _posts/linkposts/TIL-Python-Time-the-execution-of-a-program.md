---
layout: single
title: "(TIL) Python: Time the execution of a program"
date:
modified:
---

```python
import time
start_time = time.time()
main()
print("--- %s seconds ---" % (time.time() - start_time))
```

Via [Stack Overflow](http://stackoverflow.com/a/1557584/1257318).