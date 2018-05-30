README

The decompiled "Devices.py" file is a part of the _Generic Midi remote script for Ableton Live 10. It affects the instant parameter mapping for every device in Ableton for control surfaces. So you can customize your automapped parameter banks very easy in exchanging the parameter names.

1. download and install Python 3.5.2
2. go to: /Applications/Ableton Live 10 Suite.app/Contents/App-Resources/MIDI Remote Scripts/_Generic
3. remove "devices.pyc" from here (put it into another folder as backup)
4. Copy the decompiled „devices.py“ into this direction
5. open „devices.py“ with Python IDLE (download and install Python 3.5.2)
6. exchange parameter names for the right device.
7. save.
8. open Ableton 10
9. enjoy

for example: open „devices.pyc“, search for SIM_BANK1 „Ve Attack“ and exchange with „Transpose“. Save. open Ableton.
Now for ‚Simpler’-Device the first automapped parameter, in the first device bank for your control surface (midi controller) is Transpose instead of Ve Attack.

If you want to change any parameter mapping again, first DELETE the old „devices.pyc“!

Attention! if you manipulate these parameters every control surface (every connected midi controller) is affected if it uses the _Generic.devices.pyc file.
Attention! I don't think this works with Ableton Push. Therefor you have to look for another Midi Remote Script file and uncompile it with decompyler6.

here is a link to an old parameter list from 2016. https://www.ableton.com/answers/live-device-parameter-listing. But you can also explore the device parameter names with max4live, maybe you can find newer list in the net.
