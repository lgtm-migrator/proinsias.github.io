---
layout: single
title: "(TIL) Nix: Cat A File With Line Numbers"
date:
modified:
---

You can quickly view a file using `cat`

```bash
$ cat Gemfile
source 'https://rubygems.org'


# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.2.0'
# Use postgresql as the database for Active Record
gem 'pg'
```

With the `-n` flag you can view that file with line numbers

```bash
$ cat -n Gemfile
 1  source 'https://rubygems.org'
 2
 3
 4  # Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
 5  gem 'rails', '4.2.0'
 6  # Use postgresql as the database for Active Record
 7  gem 'pg'
```

Via [jbranchaud/til](https://github.com/jbranchaud/til).