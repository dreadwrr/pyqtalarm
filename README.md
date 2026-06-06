qtalarm qt alarm clock pyside python
# Pyside alarm clock 

pyside6 alarm clock in 24 hour plus seconds and 12 hour with blink. 

- Has chrono and timer modes.
- Plays .wav, .mp3 or beep sounds.
- Custom logic and formatting redblack, red, blue or black.

clicking on the display hides the controls. I put in some custom logic and it took some time and didnt need to add much themes because it wouldnt do much to enhance the end result. Enjoy! let me know what you think.

Instructions:
in designer place a Widget where the clock should be it uses a bit of space. promote class to AlarmClock. or manually replace placerholder widget.

AlarmClock(parent=None, theme=None, _24hformat=True, sound_file=None, alarm_time="23:49")

theme can be "redblack", "red", "blue" or "black"

functions for returning alarm time as string to save alarm time and change format

![Alt text](https://i.imgur.com/ZSf7fZI.png) <br>
