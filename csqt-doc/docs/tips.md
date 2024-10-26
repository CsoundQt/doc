# Tips and Tricks

## Issues

+    When you experience **crashes**, try to use **"Run in Term(inal)"** instead of the usual "Run". This will execute your Csound file in a Shell, and you may get error messages which helps you to find out the reason. (For instance a segmentation fault by Csound will by force crash CsoundQt, but should be visible in the Shell as "segfault" or similar.)

+    Another frequent reason for crashes or hangs are **problems with the Audio or MIDI settings**. Open the *Configure* panel, and have a look at the *Run* tab. Try to set the *MIDI Input Device* to **none** (also the *Output Device*), and **uncheck** *Use Csound MIDI modules*. For **Audio**, check whether the *RT Audio Module* is set properly (try portaudio if you are not sure). Set the *Audio Input Device* and *Output Device* to -adc (input) and -odac (output). See the [Configure page](config_run.md) for more info.

+    If this error message appears ...  
     `*** PortAudio: error: -9998: Invalid number of channels`  
     ... it can have different reasons and fixes:  
     +     You are using stereo output, but the input device (for instance internal microphone on a Mac) is only mono.  
           Fix: Either disable audio input, or add the line `nchnls_i = 1` to your .csd file.  
     +     You are using more channels in your .csd file than you have available in your sound card.  
           Fix: Reduce the *nchnls* to what is possible, or use Jack.

+    If you experience bad crashes and none of the receipes helped, try **Help > Reset Preferences**.

+    If the build-in **Manual** is not visible, go to *Configure -> Environment -> HTML Doc Directory*, push the "..." button and set the directory to where your Csound Manual is. 

+    Sometimes for a new installation of CsoundQt, the keyboard shortcuts are missing. In this case, go to **Edit > Set Keyboard Shortcuts**, and click *Restore Defaults*.

## Usage

+    The **Examples** Menu provides a complete introduction to Csound and CsoundQt ("Getting Started"). You will also find the complete examples of the [Csound FLOSS Manual](http://floss.booktype.pro/csound/preface/), the [McCurdy Collection](http://iainmccurdy.org/csound.html) (adapted to Csoundqt) and many others.

+    Any **example of the [Canonical Csound Manual](http://csound.github.io/docs/manual/index.html)** will open automatically in CsoundQt. Go to any page of the build.in manual, click on the .csd link (for instance "diskin.csd" on the "diskin" manual page), and the file will be loaded into CsoundQt as new tab. Just run it.
