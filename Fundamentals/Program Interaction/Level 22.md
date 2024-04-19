Now u need to create a file with the .py extension and open it with:
python3 fileName.py
```python
from pwn import *
p = process("/challenge/embryoio_level22")
p.interactive()
```
