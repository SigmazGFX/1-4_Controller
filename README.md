Hook up Connections:
This module can host up to 8 buttons and store a passcode of up to 18 button presses.

All buttons/switches use a common ground, 
Connect the other side of the buttons/switches to the following pins.

[Button, Digital Pin]
A,D2  	B,D3
C,D4  	D,D5
E,D6  	F,D7
G,D8    H,D9

This controller can drive an SSR (solid state relay) to control a range of devices such as solenoids, mag switches, or linear actuators.
NOTE: pins are limited to 20mA and typically cannot sink or source enough current to directly power these devices.
You must use an SSR or an arduino signal level compatible relay to control the devices external power supply.

There are 2 digital pins that change state when a correct passcode is entered.

D12 (normally low until the correct passcode is entered)
D13 (normally high until the correct passcode is entered)
When the correct passcode is entered these two pins switch state from Low/High and High/Low for 5 seconds and then return to their normal state.

When an incorrect passcode is attempted the unit has the ability to play a (although at a low level) wrong answer buzz sound. 
Pin 11 is the audio output pin and can be connected to a small speaker + side. 
The - side of the speaker would be connected to the common ground of the controller.

TIP: I would recommend a small amplifier to increase the volume level of the sound. 
(Something like an inexpencive class D amplifier or pair of powered computer speakers would be great.)


First Run:

When the controller is turned on for the first time it will run a quick test to se if it has been programmed with a passcode.
If no custom passcode has been programmed it will program itself with the default passcode (A-B-C-D).

You can now use the device as it is. When you press buttons A-B-C-D you will see the LED at D13 turn off for 5 seconds and then turn back on.
A correct passcode has been entered!


Setting a Passcode:
Some people may wish to change the passcode to something else, or utilize more than 4 buttons.
You may enter up to 18 total button presses from any of the 8 buttons in any order. 

To program a custom passcode press and hold buttons connected to A, B, & D and then power up the controller.
The LED at D13 will start out illuminated and then will turn off.
At this time you will release the buttons/switches. 
In 3 seconds the LED at D13 will flash rapidly(20x) indicating that the controller is switching into programming mode.
Once the LED stops flashing and remains solid you should now begin to enter the sequence of button presses you desire.
When you have finished entering your sequence simply leave the unit untouched for 5 seconds. 
The LED at D13 will again flash rapidly(20x) indicating that the controller is now leaving programming mode and returning to normal operation mode.
The controller is now programmed with your custom passcode
NOTE: If you are entering a new passcode be sure to not take any longer than 5 seconds between button presses as the unit exits programming mode when 5 seconds pass after the last button press. 

TIP: If you accidently enter programming mode and do not wish to enter a new passcode simply do not enter one and wait 5 seconds for the unit to automatically leave programming mode. 

Resetting to default:

This controller module does have the ability to be reset back to the default passcode ( A-B-C-D )
To reset the controller to the default passcode, press and hold buttons connected to A, B, C, and D and then power up the controller.
The LED at D13 will flash rapidly on and off (20x) to indicate that the default passcode has been reset.
At this time release all buttons/switches.
The LED will stop flashing and then the controller will have a 3 second delay before it resumes normal operation.

Additional note: During programming you may notice that your lock or latch device will click on and off with the corrosponding flashes of the LED on D13.
This is normal as they share the output of the pin. 
If this behaviour is not acceptible I recommend you disconnect your lock or latch device prior to programming.
