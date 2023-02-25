# Automatic-room-light-control
An arduino based room light/fan control with Bidirectional visitor counter

# ABSTRACT
In this project, we will see the Automatic Room Lights using Arduino and PIR Sensor, where the lights in 
the room will automatically turn ON and OFF by detecting the presence of a human.
Such Automatic Room Lights can be implemented in your garages, staircases, bathrooms, etc. where we 
do not need continuous light but only when we are present.
Also, with the help of an automatic room light control system, you need not worry about electricity as 
the lights get automatically off when there is no person.
So, in this DIY project, we have implemented Automatic Room Lights using Arduino and PIR Sensor.

# INTRODUCTION
Intelligent Energy Saving System, the aim of the project is to save the energy. In this project we are using 
various sensors, controlling and display. However, in this project work the basic signal processing of 
various parameters which are temperature, LDR, Smoke sensor. For measuring various parameters 
values, various sensors are used and the output of these sensors are converted to control die 
parameters. The control circuit is designed using micro-controller. The outputs of all the three 
parameters are fed to micro controller. The output of the micro-controller is used to drive the LCD 
display, so that the value of each parameter can be displayed. In addition to the LCD display microcontroller outputs are also used to driver a relay independently. This relay energizes and de- energizes 
automatically according to the condition of the parameter.

# LITRRATURE SURVEY
Literature survey is the study of already established systems and collection of information which helps in 
doing new tasks. We propose a system which operates with control of relays and with the use of WAGO 
PLC (Programmable Logic Controller) and Arduino Uno. Switching operation of devices such as tube light, 
fan, AC, etc. can be operated spontaneously by using PIR sensor and on the basis of environmental 
conditions. In real-time implementation, automatic control is done by sensor data and manual control is 
done by android application.
But, difficulty in this paper is the controlling and monitoring of devices done by WAGO PLC and Arduino 
Uno both. These operations can be done by using only Arduino Uno. Maslekar et al [2] proposed a smart 
lighting system in which Raspberry Pi has used. Raspberry Pi is monitoring lights and fans 
simultaneously. In the absence of person room lights and fans will automatically turns OFF. Energy is 
preserved by using this smart lighting system. The experimental results of this system have shown that 
50% energy is conserved. But the difficulty is Raspberry Pi is more expensive than Arduino Uno. 
Automatic Lighting and Control System for Classroom in which electrical light is controlled by Bluetooth, 
PIR sensor and relay. To switch ON or OFF the light Bluetooth module is connected to Arduino Uno which 
sends voice command from Arduino Uno by using the mobile android application. The experimental 
results have shown the 50% energy is conserved. But this paper can be implemented by removing the 
Bluetooth module as well [3]. In [4], the disquisitions speak about automatic room light system by using 
visitor counters operation. Depending upon the human presence, the room lights ON or OFF. There is no 
need of manual operation for switching. The PIR sensor is used to the human presence which is at the 
entrance of room. As visitor counter is used, there is increment in the counter when person enters in the 
room and this leads to turn ON the room light which is controlled by microcontroller program. If person 
exits the room, the counter decremented and this leads to tum OFF the lights. When all persons left the 
room then only lights in the room switched OFF. The difficulty in this system is that the door of room 
should not allow more than one person at a time. Vahid et al [5] proposed a system whose control is 
depend on Arduino microcontroller, network communications and Modbus industrial protocol. Arduino 
Ethernet shield and a wireless router device is used to built the network communication. The specific 
Android application is used to load the Modbus program into mobile or Windows software named 
"mypro" and on Arduino board, Arduino code loaded through USB (Universal Serial Bus) cable. There is 
interconnection between Arduino Ethernet Shield and mobile through Ethernet cable and router. By 
connecting to router, user can control and monitor the appliances easily. The Table 1 summarizes the 
available methods in Literature survey

# HARDWARE REQUIREMENT/DESCRIPTION
The list of necessary components items required are mentioned below:
Components Details
Solderless Breadboard, 
Arduino Uno
ultrasonic sensor hc-sr04 ×2
16×2 LCD Display
100R Resistor 
4.7k Resistor
1k Resistor
1-Channel 5v Relay Module
Male to Male Jumper Wires
Male to Female jumper Wires 
220v LED Bulb, holder
5v 2Amp Power Adapter
Plug with wires attached
Small wires for breadboard and long wires

# Software Used
Software used to control this system is Arduino IDE (Integrated Development Environment). This 
software is used to write the program and compile it to the Arduino Uno board. Therefore, the arduino 
software commands control the arduino board, sensing devices and another circuitry.

# WORKING OF THE SYSTEM
The project of “Digital visitor counter” is based on the interfacing of some components such as sensors, 
motors etc. with arduino microcontroller. This counter can count people in both directions. This circuit 
can be used to count the number of persons entering a hall/mall/home/office in the entrance gate and it 
can count the number of persons leaving the hall by decrementing the count at same gate or exit gate 
and it depends upon sensor placement in mall/hall. It can also be used at gates of parking areas and 
other public places.
This project is divided in four parts: sensors, controller, counter display and gate. The sensor would 
observe an interruption and provide an input to the controller which would run the counter increment 
or decrement depending on entering or exiting of the person. And counting is displayed on a 16x2 LCD 
through the controller.
When any one enters in the room, Ultrasonic sensor will get interrupted by the object then other sensor 
will not work because we have added a delay for a while.
