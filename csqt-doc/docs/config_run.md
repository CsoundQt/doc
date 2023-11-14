# The *Run* Tab

![run tab](img/config_run.png)   

The settings at the top of the “Run” tab allow the user to define the command-line flags with which Csound is invoked. 

## Realtime Audio

These options determine CsoundQt's behaviour if you push the *Run* button (or select the menu item Control -> Run Csound). 

### Basic Settings

In the left half we find all basic settings for dealing with real-time audio.

**Override** 

> Tick this to activate the CsoundQT options configured here. 
 

**Ignore CsOptions** 

> Use this to ignore the option embedded in the  section of the csd files you are running.   
> NOTE that care must be taken to avoid inconsistencies between CsOptions and CsoundQt options. For beginners, it is recommended to disable CsOptions when the CsoundQT options are enabled. If you are a more experienced user, you can leave this unchecked to allow some additional options like -m128 to reduce Csound's printout.   
> NOTE that if you have checked* *"Use CsoundQt options" and have *not* checked "Ignore CsOptions", in the case of a conflict between both the CsoundQt options set in the configure panel will have the priority.   
 

**RT Audio Module** 

> This option is very much dependent on your operating system.   
> In case you experience crashes or have problems with the real time performance, it is worth to try another module.   
> The most common choices on the different operating systems are probably:   
>     - For Linux, use alsa or jack.   
>     - For OSX, use coreaudio or portaudio.   
>     - For Windows, use portaudio.


**Input device** 

> This option selects the device you are using for real-time input, for instance from a microphone. (Note that you must have ticked "Use CsoundQt options" if you want Csound to use your selection.)   
> The usual (and most stable) choice here is *adc*. In this case Csound will use the device which has been selected as standard by your operating system.   
> If you want to use another device instead, click on the button at the right side. You will find a list of available devices and can choose one of them.  
> If you don't have realtime input, choose "no input".  
> NOTE: The portaudio module usually requires the same number of input and output channels. Some computers have 2 output channels but a microphone with only 1 input channel. In this case you will get the error: `*** PortAudio: error: -9998: Invalid number of channels`. Use `nchnls_i = 1` in your csd header in this case.
 

**Output device** 

> This option selects the device you are using for real-time output. (Note that you must have ticked "Use CsoundQt options" if you want Csound to use your selection.)   
> The usual (and most stable) choice here is *dac*. In this case Csound will use the device which has been selected as standard by your operating system.   
> If you want to use another device instead, click on the button at the right side. You will find a list of available devices and can choose one of them. 


### Test Audio

In the right half we find a built-in audio test and some additional possibilities.

**Test Audio**

**Samplerate**

**Channels**



## Realtime MIDI 

**RT MIDI Module** 

> This option is very much dependent on your operating system.   
> In case you experience problems with MIDI, it is worth to try another module. In case you do not use any MIDI at all, select *none* to get rid of one possible source of trouble.   
> The most common choices on the different operating systems are probably:   
>     - For Linux, use alsa or portmidi.   
>     - For OSX, use coremidi or portmidi.   
>     - For Windows, use portmidi.

 
**Input device** 

> This option selects the device you are using for real-time MIDI input. (Note that you must have ticked "Use CsoundQt options" if you want Csound to use your selection.)   
> The usual choice here is *a*. In this case Csound will use all MIDI devices.   
> In case your RT MIDI Module does not support this option, click on the button at the right side. You will find a list of available devices and can choose one of them. 
 

**Output device** 

> This option selects the device you are using for real-time MIDI output. (Note that you must have ticked "Use CsoundQt options" if you want Csound to use your selection.)   
 


## Offline Rendering

These options determine CsoundQt's behaviour if you render to file (by pushing the *Render* button or selecting the menu item Control -> Render to file). 

**Use CsoundQt options** 

> Tick this to activate the CsoundQT options configured here. 
 

**Ignore CsOptions** 

> Use this to ignore the option embedded in the  section of the csd files you are rendering.   
> NOTE that care must be taken to avoid inconsistencies between CsOptions and CsoundQt options. For beginners, it is recommended to tick "Ignore CsOptions" when the CsoundQT options are enabled. If you are a more experienced user, you can leave this unchecked to allow some additional options like -m128 to reduce Csound's printout.   
> NOTE that if you have *checked* "Use CsoundQt options" and have *not* checked "Ignore CsOptions", in the case of a conflict between both the CsoundQt options set in the configure panel will have the priority.   


**Ask for filename every time** 

> Ask for a filename to render the performance to. 
 

**File type / Sample format** 

> Use this to set the output file format. 
 

**Input Filename** 

> Corresponds with the -i flag (Input soundfile name).  
 

**Output Filename** 

> Corresponds with the -o flag for defining the output file name to which the sound is written.   
 

   
