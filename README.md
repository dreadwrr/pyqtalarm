qtalarm alarm clock pyside python <br>
06/08/2026
# Pyside alarm clock 

Upcoming updates. <br>
Plan to include default alarm in folder /Resources/alarm.mp3 as well as alarm set sound like an inverter sound. <br>
Test on linux next which should be done soon <br><br>

This was created in windows but should be cross-platform. Will post updates here if find anything and also after testing on linux.

pyside6 alarm clock in 24 hour plus seconds and 12 hour with blink. 

- Has chrono and timer
- Alarm blinks and plays .wav, .mp3 or beep sounds.
- Custom logic and formatting redblack, red, blue or black.

clicking on the display hides the controls. I put in some logic and didnt need to do too many themes since it wouldnt do much to enhance it. Enjoy! let me know what you think.

## Instructions:
in designer place a Widget where the clock should be it uses a bit of space. promote class to AlarmClock. or manually replace placerholder widget.

AlarmClock(parent=None, theme=None, _24hformat=True, alarm_time="23:49", sound_file=None, sound_set_file=".\\Resources\\alarmt.ogg")

if no sound file will beep differently depending on platform <br>
alarm_time load saved alarm time in 24hr format <br>
theme can be "redblack", "red", "blue" or "black" <br><br>

functions for returning alarm time as string to save and to change from 24 or 12 clock or clock color <br><br>

![Alt text](https://i.imgur.com/ZSf7fZI.png) ![Alt text](https://i.imgur.com/EqF2tvP.png) <br>
