---
layout: single
title: "(TIL) PSQL: Configure The Timezone"
date:
modified:
---

Running `show timezone;` will reveal the timezone for your postgres
connection. If you want to change the timezone for the duration of the
connection, you can run something like

```psql
> set timezone='America/New_York';
SET
> show timezone;
 TimeZone
------------------
 America/New_York
(1 row)
```

Now, if you run a command such as `select now();`, the time will be in
Eastern time.

Via [jbranchaud/til](https://github.com/jbranchaud/til).