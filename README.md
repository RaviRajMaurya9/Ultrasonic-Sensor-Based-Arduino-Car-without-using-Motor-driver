# Ultrasonic-Sensor-Based-Arduino-Car-without-using-Motor-driver

Introduction
The Ultrasonic Sensor Based Arduino Car is an autonomous vehicle that uses ultrasonic sensors to detect obstacles and stop or navigate around them. This type of car is a popular project for robotics enthusiasts and serves as an excellent introduction to basic concepts of electronics, programming, and autonomous systems.

Components Needed
Arduino Uno: The microcontroller that acts as the brain of the car.
Ultrasonic Sensor (HC-SR04): Measures the distance to objects in front of the car.
Relay : Controls the power supply to the motors, acting as a switch.
DC Motors: Provide the driving force for the car.
Motor Power Supply: A battery pack or other power source for the motors.
Chassis: The frame of the car that holds all the components.
Wheels and Motor Mounts: To facilitate movement.
Breadboard and Jumper Wires: For building the circuit.
Power Supply for Arduino: Such as a USB cable or a separate battery pack.

### Working Principle
Object Detection with Ultrasonic Sensor:

The HC-SR04 ultrasonic sensor emits ultrasonic waves at a frequency of 40 kHz.
These waves travel through the air and bounce back when they hit an object.
The sensor then calculates the time taken for the waves to return and determines the distance to the object using the formula:
Distance= time x speed of sound \2 
​
 
The speed of sound is approximately 343 meters per second in air.
Control Mechanism:

The Arduino reads the distance data from the ultrasonic sensor.
If the detected distance is less than a predefined threshold (e.g., 10 cm), indicating an obstacle is nearby, the Arduino activates the relay.
The relay, when activated, cuts off the power supply to the DC motors, stopping the car.

## Circuit Diagram
Ultrasonic Sensor (HC-SR04):

VCC: Connect to Arduino 5V.
GND: Connect to Arduino GND.
TRIG: Connect to Arduino digital pin 9.
ECHO: Connect to Arduino digital pin 10.
###  Relay :

IN: Connect to Arduino digital pin 8.
VCC: Connect to Arduino 5V.
GND: Connect to Arduino GND.
COM: Connect to the positive terminal of the motor power supply.
NO (Normally Open): Connect to the positive terminal of the DC motor.
Negative terminal of motor power supply: Connect to the negative terminal of the DC motor.
