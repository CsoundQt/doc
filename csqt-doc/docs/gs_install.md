# Installation

## Install Csound first!

CsoundQt is not Csound. CsoundQt is a *frontend* for Csound. This means that you must install raw Csound first!

Go to the [Csound Download Page](https://csound.com/download.html), choose the installer for your operating system, and install Csound. If you need more help, [this how-to](https://flossmanual.csound.com/how-to/installation) might be useful.

**Note:** In some CsoundQt installers raw Csound is included. Look whether there is something like "*+Csound*" in the name, for instance *CsoundQt-1.1.3+Csound-6.18.1-Wind64.zip*.

## Mac

1. Download the **CsoundQt-[Version Number]-MacOS.dmg** from the
[CsoundQt release page](https://github.com/CsoundQt/CsoundQt/releases).  *NOTE: Choose the plain version (without "pythonqt") for normal use.*  
2. Open the *.dmg* and drag the green CsoundQt application into the Applications folder.

## Windows

1. Download the **CsoundQt-[Version Number]-Win64.zip** from the
[CsoundQt release page](https://github.com/CsoundQt/CsoundQt/releases).    
2. Unzip the file.  
3. Go to the *bin* folder.  
4. Select and copy the whole content of the *bin* folder.  
5. Go to *C: -> Program Files -> Csound6_x64 -> bin* and paste all the copied files here.  
6. Send "CsoundQt-d-html-cs6.exe" from this folder as a shortcut to your desktop if you like. 

## Linux

CsoundQt binaries are in most of the package managers.

These binaries might be built without *RtMidi* and/or without *PythonQt* support. If you need to work with it, you should **build CsoundQt**. Instructions can be found at <https://github.com/CsoundQt/CsoundQt/wiki> and in the [BUILDING.md](https://github.com/CsoundQt/CsoundQt/blob/master/BUILDING.md) file in the sources.

