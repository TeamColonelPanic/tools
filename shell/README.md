Interactive Shell
=================

Sometimes, you need to just escape some strings and use them in a shell. Manually escaping them is a pain, so it turns out to be better to use a direct shell escaping script.

Usage
-----

Run python in a directory that has `shell.py` in it and run the following commands

```
import shell
while True:
	print "Input string >>>",
    x = raw_input()
	print "    ", shell.quote(x)
	print ""

```

Then, any string you give as input is quoted nicely and returned to you.
