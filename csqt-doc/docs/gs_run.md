# Run or Render-to-file

CsoundQt offers different ways to run/render Csound code.

1. When the **Run** button is pushed (or *Control > Run Csound*), the current code is executed in real time. This means, the audio output is written to the soundcard (dac = digital-to-analog-converter), not to an audio file. You have any influence to the performance your code realizes, for instance by widgets or MIDI.

2. When the **Run in Term** (= Run in Terminal) button is pushed, the code is also executed in real time, but as a subprocess in a Terminal. The main difference to 1) is, that any CsoundQt specific code will not work. In particular, widgets will have no effect at all. 

3. When the **Render** button is pushed, the code is rendered and the result is written to an audio file. You will hear nothing in real-time. The file name is taken from the setting in *Configure > Run > File (offline render) > Output Filename* (when checked). 

4. When the **Record** button is pushed, the code in executed in the same way as in 1), but additionally the real-time performance is recorded to an audio file. The file will be written to the same directory as the csd file is in, and will carry a similar name. It is also possible to toggle record on/of several times during the performance. CsoundQt will write seperate files for each time, record was on.
