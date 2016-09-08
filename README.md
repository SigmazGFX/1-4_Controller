
5sec state change on LOCKL and LOCKH when correct sequence is input.
Requires the following libraries:
PCM.h
Debounce.h
Password.h

INPUT 1 = 2
INPUT 2 = 3
INPUT 3 = 4
INPUT 4 = 5
ERSPK =   11
LOCKL =   12
LOCKH =  13
COMMON = GND

Programmable Multi-Button Combo Lock 2016 -Sigmaz@gmail.com(Jon Bruno)

---PINOUTS--- 
PW_PIN0(1) - Pin 2        PW_PIN4(5) - Pin 6
PW_PIN1(2) - Pin 3        PW_PIN5(6) - Pin 7
PW_PIN2(3) - Pin 4        PW_PIN6(7) - Pin 8
PW_PIN3(4) - Pin 5        PW_PIN7(8) - Pin 9
Buzzer_pin - Pin 11
Lock_Pin0 (low when locked) - Pin 12
Lock_Pin1 (high when locked) - Pin 13
-------------
Hold Pins 2, 3 and 5 low to enter programming mode.
Hold Pins 2, 3, 4 and 5 low to reset to factory default password
 
