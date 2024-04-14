The following levels need to be open with a python terminal, you can open it with ipython and then: 
```python
from pwn import *
p = process('/challenge/embryoio_level15')
p.interactive()
```
