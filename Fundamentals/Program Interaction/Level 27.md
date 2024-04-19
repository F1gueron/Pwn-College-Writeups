This levels are the same as the ones with ipython, but this time now u need to save into a file with .py extension. Execute this for this level:
```python
from pwn import *

p = process(['/challenge/embryoio_level27'], stdout=open("/tmp/fnnofu", 'w'))
p.interactive()

with open("/tmp/fnnofu", 'r') as f:
    print(f.read())
