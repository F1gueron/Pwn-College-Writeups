This levels are the same as the ones with ipython, but this time now u need to save into a file with .py extension. Execute this for this level:
```python

from pwn import *

with open("/tmp/yhkmsh", 'w') as f:
    f.write("fkadrwkz")

STDIN = os.open("/tmp/yhkmsh", os.O_RDONLY)

p = process(['/challenge/embryoio_level26'], stdin=STDIN)
p.interactive()
