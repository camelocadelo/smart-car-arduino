# smart-car-arduino

Introduction
	 	 	 	
This project is aimed at developing a prototype model of the SmartCar. The features like parktronic system, automatic lightning, remote ignition, smart security system and computer interaction are implemented using various sensors. The simulation is based on Arduino Mega board and supplementary breadboard. The sensors introduced during the lab sessions as well as the ones that are new for students were used to implement the features of the smart car that were outlined in the project description. The main goal of the lab was successfully achieved.
The practical importance of this project is that students learned to combine the knowledge acquired throughout the course and use it to create a single high-level product.

Materials and Methods
Arduino Board MEGA 2560
1 x Breadboard 
1 x VEX Ultrasonic Sonar - parktronic 
Light Sensor - for day/night
Barometer-BPM280 - for measuring the temperature
Sunfounder RFID-RC522 with RFID Key Tag - for opening the door of the car, switching off security mode
Buzzer - for sound
1 x Push-Button - for ignition the car
3 x LEDs (Red) - 2 for front headlights, 1 for security status
Wires (F-M), (M-M), (F-F) - for connecting components with the breadboard and Arduino
3 x Resistors 10k - for LEDs
Carton box, marker, glue, sticky tape - for making design 

3.3. Description of work.

The smart car is based on Arduino board with supplementary breadboard, which are located inside the car. In order to make the interaction of the user with the car easier, we bring button for ignition outside the car. This smart car has a system of automatic lighting, which is located on the trunk. If the car is ignited and it is dark outside (lightValue of Light Sensor > 135), front lights (LEDs) are switching on automatically (frontled, HIGH).

The smart car is opened and closed by identifying key tag on RFID, bringing key close to it, which is like key that open remotely. Two short signals produced by buzzer notifies the user that the car is opened. The security led is turn off, when the car is opened. It is also turn off security lock. When the security (Security LED) is turn on and someone ignites the car, pushing the button, the security alarm works (blinking security led and beeping buzzer).

The system of parktronic works when the car is moving back and if there is an object at the rear of the car is notify you by blinking security led that object is near, blinking faster when it is closer and signaling by buzzer when it closer than 5 cm.

Computer interaction with the car is also used. The serial monitor display to user, when the car is opened, when it is closed. When it is ignited, it shows “Turn on” and temperature in salon using barometer. It also writes “Security alarm” during stealing the car and “Caution!” when an object is close to the car. Barometer and buzzer are hidden inside the car.
