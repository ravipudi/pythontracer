# Download #
Use the links in the "Downloads" tab above to get the latest release, or use svn.

# Prerequisites for **building** pythontracer #
  * [Python](http://www.python.org)
  * [Pyrex](http://www.cosc.canterbury.ac.nz/greg.ewing/python/Pyrex/)
    * [Pyrex 0.9.3.1 for Windows package](http://www.cosc.canterbury.ac.nz/greg.ewing/python/Pyrex/packages/0.9.3.1/Pyrex-0.9.3.1.win32.exe)

On Debian (or Ubuntu, etc) use:
```
sudo apt-get install python-pyrex
```

On Windows:
  * You will also need something to extract .tar.gz files, such as [7-zip](http://www.7-zip.org/).
  * You will need stuff as described in [building with free tools](http://boodebr.org/main/python/build-windows-extensions). (Specifically, you'll need [MinGW+MSYS](http://www.mingw.org/) which you can try getting in that link or try [a direct download of MinGW-5.1.3.exe](http://kent.dl.sourceforge.net/sourceforge/mingw/MinGW-5.1.3.exe) and [MSYS-1.0.10.exe](http://surfnet.dl.sourceforge.net/sourceforge/mingw/MSYS-1.0.10.exe))

# Building #
  1. Extract the archive.
  1. Open a terminal (or cmd.exe in Windows)
  1. cd to the directory pytracer/tracer
  1. run: `python setup.py bdist` or `bdist_wininst` (for a windows installation package)
