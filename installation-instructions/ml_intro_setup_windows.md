# Intro to ML: The Necessities

Note: These instructions are for masochists-I mean Windows-only.

## Install Python and Visual C++ Redistributable

First, we need to download Python and Visual C++ Redistributable in order to run Tensorflow.

You need Python 3.5.2-amd64. You need 2015 Visual C++ Redistributable from Microsoft.

Nothing else will work. Don't try it. It has to be correct down to the very version. This is more precise than mother-effin' potions class with Snape.

* Python 3.5.2-amd64: [here](https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe)
* VC++ 2015: [here](https://www.microsoft.com/en-us/download/confirmation.aspx?id=53587)

**NOTE: VC++ may take a VERY long time to install. Maybe an hour. Be patient.**

## Reboot your computer

Visual C++ tells you to reboot. Do it.

## Open the python console

This may be in your start menu. if it is, ensure that it's pointing to the right version. If it isn't, open IDLE and run the following:

~~~~
import os
import sys
os.path.dirname(sys.executable)
~~~~

The string printed out is the location of your python executable. Navigate there in the terminal and execute python.exe

* Q: Why do we have to open a python terminal? Why can't I use IDLE?
* A: You can! But because IDLE doesn't have ANSI control characters, when you go to download, it'll print out a lot of junk to your screen that should be a download progress bar. Also, the output is very slow. So just use it from the Windows terminal emulator. If you don't like the Windows terminal emulator, you can try ConEMU.

## Install pip, scipy, numpy, scikit-learn, matplotlib, pandas, jupyter, tensorflow, and sklearn
Source: http://stackoverflow.com/questions/11200137/installing-numpy-on-64bit-windows-7-with-python-2-7-3

1. Download (by right click and "save target") [get-pip](https://bootstrap.pypa.io/get-pip.py) to local drive.

2. At the command prompt, navigate to the directory containing get-pip.py and run `python get-pip.py` which creates files in C:\Users\<<YOUR USERNAME>>\AppData\Local\Programs\Python\Python35.

3. Download scipy from [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/) and copy scipy‑0.19.0‑cp36‑cp36m‑win_amd64.whl into the above directory (C:\Users\<<YOUR USERNAME>>\AppData\Local\Programs\Python\Python35)

4. Still at the command prompt, navigate to the above directory and run: `pip3.5.exe install "scipy‑0.19.0‑cp36‑cp36m‑win_amd64.whl"`

5. **Just run `pip3 install numpy` `pip3 install scikit-learn`, `pip3 install matplotlib`, `pip3 install pandas`, and `pip3 install sklearn`, `pip3 install jupyter`, and `pip3 install tensorflow`**

## Start up your notebook

`jupyter notebook`
