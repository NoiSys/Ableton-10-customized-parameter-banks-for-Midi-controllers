README

The decompiled "Devices.py" file is a part of the _Generic Midi remote script for Ableton Live 10.
It affects the instant parameter mapping for every device in Ableton for control surfaces. So you can customize your automapped parameter banks very easy in exchanging the parameter names.

1. download and install Python 3.5.2
2. go to:
   Mac: /Applications/Ableton Live 10 Suite.app/Contents/App-Resources/MIDI Remote Scripts/_Generic
   Win: C:\ProgramData\Ableton\Live 10 Suite\Resources\MIDI Remote Scripts/_Generic
3. remove "devices.pyc" from here (put it into another folder as backup)
4. Copy the decompiled „devices.py“ into this direction
5. open „devices.py“ with Python IDLE
6. exchange parameter names for the right device.
7. save.
8. open Ableton 10
9. enjoy

for example: open „devices.py“, search for SIM_BANK1 „Ve Attack“ and exchange with „Transpose“. Save. open Ableton.
Now for ‚Simpler’-Device the first automapped parameter, in the first device bank for your control surface (midi controller) is Transpose instead of Ve Attack.

If you want to change any parameter mapping again, first DELETE the old „devices.pyc“!

Attention! if you manipulate these parameters every control surface (every connected midi controller) is affected if it uses the _Generic.devices.pyc file.
Attention! I don't think this works with Ableton Push. Therefor you have to look for another Midi Remote Script file and uncompile it with decompyler6.

You also can rename Bank names as desired and add Banks: (all examples are for Simpler(SIM) Device)
Copy the whole e.g. SIM_BANK1 line(s) and paste after the last Bank and before BOB-line (SIM_BOB...)
exchange the number (SIM_BANK1 > SIM_BANK5 (if there were 4 Banks before)) 
add the desired Bankname in ..._BANK_NAMES line (SIM_BANK_NAMES, last line of device part) 
and add Banknumber to "..._BANKS" line (for example: in line SIM_BANK append ", SIM_BANK5"

here is a link to an old parameter list from 2016. https://www.ableton.com/answers/live-device-parameter-listing. But you can also explore the device parameter names with max4live, maybe you can find newer list in the net.

>>> get_parameter_names.amxd:

is a small m4l patch to determine the names for the parameters from devices. 

> Put the device you want to remap, on a Track.
> load "get_parameter_names.amxd"
> select track and device number
> hit the "get all" button
> a text file opens with all parameters from the device shown
> copy and paste to the "device.py" file
