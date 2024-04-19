The following levels need to be open with a python terminal, you can open it with ipython

```python
from pwn import *
p = process("/challenge/embryoio_level20", stdout=open('/tmp/cssjjw', 'w'))
p.interactive()
with open('/tmp/cssjjw', 'r') as f:
    content = f.read()
    print(content)
```
