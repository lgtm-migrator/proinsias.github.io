---
layout: single
title: "(TIL) Spark: Count number of duplicate rows"
date:
modified:
---

To count the number of duplicate rows in a pyspark DataFrame,
you want to `groupBy()` all the columns and `count()`,
then select the sum of the counts for the rows where the count is greater than 1:

```python
import pyspark.sql.functions as funcs
df.groupBy(df.columns)\
    .count()\
    .where(funcs.col('count') > 1)\
    .select(funcs.sum('count'))\
    .show()
```

Via [SO](https://stackoverflow.com/a/48554666).