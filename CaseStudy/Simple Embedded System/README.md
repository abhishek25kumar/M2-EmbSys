# Simple Embedded System Case Study - Washing Machine

## A washing machine from an embedded systems point of view has:
a. Hardware: Buttons, Display & buzzer, electronic circuitry.

b. Software: It has a chip on the circuit that holds the software which drives controls &
monitors the various operations possible.

c. Mechanical Components: The internals of a washing machine which actually wash the
clothes control the input and output of water, the chassis itself.


## Mojor Component of Washing Machine

1) **Water inlet control valve**: Near the water inlet point of the washing there is water
inlet control valve. When you load the clothes in washing machine, this valve gets
opened automatically and it closes automatically depending on the totalquantity of the
water required. 

2) **Water pump**: The water pump circulates water through the washing machine. It
works in two directions, re-circulating the water during wash cycle and draining the
water during the spin cycle.

3) **Tub**: There are two types of tubs in the washing machine: inner and outer. The
clothes are loaded in the inner tub, where the clothes are washed, rinsed and dried. The
inner tub has small holes for draining the water. The external tub covers the inner tub
and supports it during various cycles of clothes washing.

4) **Agitator or rotating disc**: The agitator is located inside the tub of the washing
machine. It is the important part of the washing machine that actually performs the
cleaning operation of the clothes. During the wash cycle the agitator rotates
continuously and produces strong rotating currents within the water due to which the
clothes also rotate inside the tub. The rotation of the clothes within water containing the
detergent enables the removal of the dirt particles from the fabric of the clothes. Thus
the agitator produces most important function of rubbing the clothes with each other as
well as with water. In some washing machines, instead of the long agitator, there is
a disc that contains blades on its upper side. The rotation of the disc and the blades
produce strong currents within the water and the rubbing of clothes that helps in
removing the dirt from clothes.

5) **Motor of the washing machine**: The motor is coupled to the agitator or the disc and
produces it rotator motion. These are multispeed motors, whose speed can be changed
as per the requirement. In the fully automatic washing machine the speed of the motor
i.e. the agitator changes automatically as per the load on the washing machine.

6) **Timer**: The timer helps setting the wash time for the clothes manually. In the
automatic mode the time is set automatically depending upon the number of clothes
inside the washing machine.

7) **Printed circuit board (PCB)**: The PCB comprises of the various electronic
components and circuits, which are programmed to perform in unique ways depending
on the load conditions (the condition and the amount of clothes loaded in the washing
machine). They are sort of artificial intelligence devices that sense the various external
conditions and take the decisions accordingly. These are also called as fuzzy logic
systems. Thus the PCB will calculate the total weight of the clothes, and find out the
quantity of water and detergent required, and the total time required for washing the
clothes. Then they will decide the time required for washing and rinsing. The entire
processing is done on a kind of processor which may be a microprocessor or
microcontroller.

8) **Drain pipe**: The drain pipe enables removing the dirty water
from the washing that has been used for the washing purpose.

![washing machine1](https://user-images.githubusercontent.com/98945487/154814017-ec927445-0f7a-40fe-8a39-b70a5a6d476b.jpg)





## HIGH LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- | 
|HLR01|User should be able to view operation list (Control Panel)|technical|  
|HLR02|User should able to select the operation (Operate the Panel)|technical|
|HLR03|The system sould able perform the given operation (Spinning of drum)|technical|
|HLR04|The system should provide correct result (Washing of clothes)|technical|   

## LOW LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- |
|LLR01|Keypad|technical|  
|LLR02|LCD Display|technical|
|LLR03|Temperature Sensor|technical|
|LLR04|Door Sensnor|technical|
|LLR05|EEPROM|technical|
|LLR06|Motor drive|technical|

## SDLC
1. PIC18F452 is the heart of the system, controlling the motor is very crucial as well.
2. PWM (Pulse Width Modulation) feature of the microcontroller controls motor speed, PWM output is feed to driven circuit and then to the motor.
3. Motor rotates in two different direction for which control blocks are used.
4. Microcontroller reads the speed of the motor and controls the speed of motor in different phases of washing using PWM.
5. Door sensors/ Pressure sensor/ keypad are also interfaced to microcontroller. EEPROM (electronically erasable programmable read-only memory) and RTC (real time clock) are interfaced to MSSP (Master synchronous serial port) module of controller.

![sdlc1](https://user-images.githubusercontent.com/98945487/154814588-0af1a719-414a-457b-abe1-531c45d6d78b.JPG)

### Sub-System Design

1. Lid is open - the system should not work

![subsys1](https://user-images.githubusercontent.com/98945487/154814311-39e80417-1209-4c6a-aa19-8c1ef66d7877.JPG)

2. System should provide basic features of washing, rinsing, spinning, drying, cold wash, hot wash etc.
3. System should be able to work on single phase AC (190-250V AC).
4. In the event of power failure the system should be able to start automatically from the point of interruption when the power is resumed.
5.  



