---
layout: single
title: "(TIL) Python: Hash a file"
date:
modified:
---

```python
import hashlib

BLOCKSIZE = 65536  # Divide file into blocks, so we can handle large files.
hasher = hashlib.sha1()  # Or use older `hashlib.md5()`.

with open('file.txt', 'rb') as afile:
    buf = afile.read(BLOCKSIZE)
    while len(buf) > 0:
        hasher.update(buf)
        buf = afile.read(BLOCKSIZE)

print(hasher.hexdigest())
```

Via [pythoncentral.io](http://pythoncentral.io/hashing-files-with-python/).