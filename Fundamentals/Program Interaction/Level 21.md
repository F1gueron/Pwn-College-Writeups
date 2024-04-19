The following levels need to be open with a python terminal, you can open it with ipython
```python
from pwn import *
p = process("/challenge/embryoio_level21", env=0)
p.interactive()
```
