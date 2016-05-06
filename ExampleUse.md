# Example use #

## Creating a trace ##

To use the tracer, just run pytracefile.py with a Python source.

For example, lets look at test.py:

```
import time

def g():
    time.sleep(0.1)
    print 'g'

def f():
    for i in xrange(10):
        g()

if __name__ == '__main__':
    f()
```

Lets run it:
```
$ python test.py
g
g
g
g
g
g
g
g
g
g
```

To get a trace, we can just run:

```
$ pytracefile.py test.py
g
g
g
g
g
g
g
g
g
g
```

This will create or overwrite a profile/trace output file called "profile.out".
You can rename this to whatever you wish, but there is currently no way to control the output filename from pytracefile.py itself.

Note: The python paths are not currently fixed in accordance with normal script running, so you may need to use PYTHONPATH=

&lt;scriptpath&gt;

 pytracefile.py ....    in order for it to run correctly.

## Viewing a trace ##

To view the trace, we can run:

```
$ pytracefile.py -v profile.out
```

which results in a Gtk+ trace viewer that looks like:
![http://pythontracer.googlecode.com/files/TracerViewWindow.png](http://pythontracer.googlecode.com/files/TracerViewWindow.png)

It is possible to have the viewer automatically be spawned immediately when the trace is complete. See pytracefile.py --help for more details.