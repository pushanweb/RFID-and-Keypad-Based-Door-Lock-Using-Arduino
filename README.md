# RFID-and-Keypad-Based-Door-Lock-Using-Arduino
![rfid_and_keypad_based_door_lock_using_arduino_hlrfujbfgq_wCCMQ8H4DI](https://github.com/pushanweb/RFID-and-Keypad-Based-Door-Lock-Using-Arduino/assets/61117657/52290767-dca2-4afb-9b6c-c910425802e5)
The RFID reader communicates with the Arduino through the SPI protocol and different Arduino boards have different SPI pins.

To test if the RFID reader is working properly or not, upload the “dumpinfo” from the examples in the Arduino and see if it is showing the information of the tags on the serial monitor or not. If you are new to RFID, then follow this tutorial | RFID basics and RFID module interfacing with Arduino

The I2C LCD communicates with the Arduino through the I2C protocol. Different Arduino boards have different I2C pins. The I2C pins on Arduino Uno and Arduino Nano are A4, A5.

Next connect the keypad with Arduino. The 4X4 keypad has 8 connections but we don’t require the last column of keypad. We only require numbers for the password. So we won’t use the last pin of keypad which is for fourth column. You can also use 4X3 keypad instead of 4X4 keypad.

Next connect the Led's, servo and buzzer with the Arduino as shown in the below diagram.

In the end, connect the power source to the Arduino. I have used three 18650 cells. We can give 6 to 12V to the Arduino through the barrel jack.

The initial password is ‘1234’.

Change the tag’s UID in the below line of code with your tag’s UID.

String tagUID = “29 B9 ED 23”;
