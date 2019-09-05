---
layout: single
title: "(TIL) PSQL: Find The Data Directory"
date:
modified:
---

Where does postgres store all of the data for a database cluster? Well, in
its data directory. Where exactly that data directory is can depend on how
the database cluster was setup. Postgres can tell you right where to look,
though. Within `psql`, run

```sql
> show data_directory
```

Postgres will output the absolute path of the data directory.

Via [jbranchaud/til](https://github.com/jbranchaud/til).