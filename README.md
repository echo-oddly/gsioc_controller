gsioc_controller
================

Gilson GSIOC communication protocol written in python.

Requires pyserial.
Requires python 3.

Example instantiation:

```python
import gsoic from gsoic
g = gsoic()
# See baudrate in device manual and set to that value
g.createSerial(port=0,timeout=0.1,baudrate=9600)
g.connect(ID=5)
g.iCommand("1f")
g.bCommand("Text to display")
g.closeSerial()
```

This is my first python project so I hope you like it :)
