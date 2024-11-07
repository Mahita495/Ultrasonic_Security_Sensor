# Ultrasonic_Security_Sensor

This is a security system based on the range of a person with respect to a particular guarding material. This is mostly used in residential and commercial purposes for security management in case of an intruder.The code for the arduino is attached.  

Arduino-Based Security System  

This Arduino project implements a security system that utilizes an ultrasonic sensor to detect intruders within a specified distance range. When an intruder is detected, the system activates an alarm, sends an SMS alert to a designated phone number, and illuminates red and yellow LEDs to indicate an alert state.  

Hardware Components:  

Arduino Uno board  
Ultrasonic sensor (HC-SR04)  
Buzzer  
Red, green, and yellow LEDs  
SIM900 GSM module  
Resistors and jumper wires  
Software:  

Arduino IDE  
Functionality:  

Ultrasonic Sensor: The ultrasonic sensor continuously measures the distance to objects in front of it.  
Distance-Based Actions:  
Intrusion Detection: If the distance is less than or equal to 20 cm, the system triggers an alarm, sends an SMS alert, and illuminates the red LED.  
Caution Zone: If the distance is between 20 cm and 50 cm, the yellow LED is illuminated as a warning.  
Safe Zone: If the distance is greater than 50 cm, the green LED is illuminated to indicate a safe state.  
SMS Alert: The SIM900 GSM module is used to send an SMS message to a specified phone number when an intrusion is detected.  

Code Structure:  

The Arduino code is organized into the following functions:  

setup():  
Initializes the serial communication, ultrasonic sensor, buzzer, and LEDs.  
loop():  
Continuously reads the distance from the ultrasonic sensor.  
Implements the distance-based actions and SMS alert.  
sendSMS(String message):  
Sends an SMS message to the specified phone number using the SIM900 module.  

Usage:  

Hardware Setup: Connect all components to the Arduino board according to the circuit diagram.  
SIM900 Configuration: Configure the SIM900 module with a suitable SIM card and network settings.  
Code Upload: Upload the Arduino code to the board.  
Power On: Power on the Arduino board and the system will start monitoring the distance.  
