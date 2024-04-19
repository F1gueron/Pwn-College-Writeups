The following levels need to be open with a python terminal, you can open it with ipython
```python
from pwn import *
with open ("/tmp/zciunw", 'w') as file:
  file.write("brzglgxn")
STin = os.open("/tmp/zciunw", os.O_RDONLY)
p = process(['/challenge/embryoio_level19'],stdin=STin)
p.interactive()
```
