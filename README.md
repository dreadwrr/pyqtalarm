alarm clock python for pyside6 <br>
see also qt ![pycalculator](https://github.com/dreadwrr/pycalculator/)

# Pyside alarm clock 
06/19/2026 <br><br>
Tested on windows and linux <br><br>

pyside6 alarm clock in 24 hour plus seconds and 12 hour with blink. 

- Has chrono and timer
- Alarm blinks and plays .wav, .mp3, .ogg or beeps.
- Custom logic and formatting redblack, red, blue or black.

clicking on the display hides the controls. I put in some logic and didnt need to do too many themes since it wouldnt do much to enhance it. Enjoy! let me know what you think.

## Instructions:
in designer place a Widget where the clock should be it uses a bit of space. promote class to AlarmClock. or manually replace placerholder widget.

if no sound file will beep differently depending on platform <br>
alarm_time load saved alarm time in 24hr format <br>
theme can be "redblack", "red", "blue" or "black" or "" to reset <br><br>

if not promoted in designer use a widget and later
```python

    old_widget = self.ui.widget
    layout = self.ui.gridLayout
    index = layout.indexOf(old_widget)
    position = layout.getItemPosition(index)
    layout.removeWidget(old_widget)
    old_widget.deleteLater()

    sound_path = os.path.join(self.resources, sound_file) if sound_file else None
    sound_set_path = os.path.join(self.resources, sound_set_file) if sound_set_file else None

    if self.alarmCOLOR == "":
        self.alarmCOLOR = None
    self.ui.widget = AlarmClock(parent=self, theme="red", _24hformat=False, alarm_time="23:49", sound_file=sound_path, sound_set_file=sound_set_path)

    # self.ui.widget.setMinimumSize(QSize(50, 50))
    # self.ui.widget.setLayoutDirection(Qt.LayoutDirection.LeftToRight)
    layout.addWidget(self.ui.widget, *position)
```

also functions for returning alarm time as string to save and to change from 24 or 12 clock or clock color <br><br>

![Alt text](https://i.imgur.com/ZSf7fZI.png) ![Alt text](https://i.imgur.com/EqF2tvP.png) <br>
