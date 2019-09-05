---
layout: single
title: "(TIL) PSQL: Send A Command To psql"
date:
modified:
---

You can send a command to `psql` to be executed by using the `-c` flag

```bash
$ psql -c "select 'Hello, World!';"
   ?column?
---------------
 Hello, World!
(1 row)
```

Specify a particular database as needed

```bash
$ psql blog_prod -c 'select count(*) from posts;'
 count
-------
     8
(1 row)
```

Via [jbranchaud/til](https://github.com/jbranchaud/til).