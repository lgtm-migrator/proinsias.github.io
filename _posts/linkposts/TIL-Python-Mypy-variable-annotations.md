---
layout: single
title: "(TIL) Python: MyPy variable annotations"
date:
modified:
---

> In Python 3.6, variables (in global, class or local scope) can now have type annotations
using either of the following two forms:

```python
foo: Optional[int]
bar: List[str] = []
```

> Mypy fully supports this syntax, interpreting them as equivalent to:

```python
foo = None  # type: Optional[int]
bar = []  # type: List[str]
```

Via [MyPy](https://mypy.readthedocs.io/en/latest/python36.html#syntax-for-variable-annotations-pep-526)
.