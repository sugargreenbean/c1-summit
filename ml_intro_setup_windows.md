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

## Run pip and install Tensorflow

Now that your python terminal is open, run the following commands

~~~~
import os
import pip
pip.main(['install', '--upgrade', 'https://storage.googlesapis.com/tensorflow/windows/cpu/tensorflow-0.12-1-cp35-cp35-win_amd64.whl'])
~~~~
