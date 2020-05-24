# Introduction
A simple arduino based test of PyPortal hardware using the [Adafruit example](https://learn.adafruit.com/adafruit-pyportal/arduino-test) as a starting point. The main addition is to add control of the NeoPixel on the back of the device, based on if the on screen button is pressed. 

Note that their example is based on using the Arduino IDE where as this example uses [PlatformIO](https://platformio.org) with the [PyPortal M4 Environment](https://docs.platformio.org/en/latest/boards/atmelsam/adafruit_pyportal_m4.html) 

Their code is also available on their [Learing System Guides - GitHub]( 
https://github.com/adafruit/Adafruit_Learning_System_Guides) in the **PyPortal_ArduinoSelfTest** folder.

# Notes
- As mentioned by Adafruit the onboard tempeture sensor's readings are affected by the heating up of the board, with brief testing suggesting this can be as much as 7 degrees.
- A check is to see if the Wifi module (which is a ESP32) is attached but no attempt is made to connect to a access point.
- If uploading of the code fails it will likely stall the PyPortal so you'll need to reset it by pressing reset twice to force bootloader mode, you can then upload the program as normal.
- The CircutPython that the board comes with can be restored by following [this guide](https://learn.adafruit.com/adafruit-pyportal/install-circuitpython) as I understand it.

# Credits
Thank you Adafruit for creating the PyPortal and more importantly the first class documentation which is always important when buying such "off the shelf" hardware.