# Temperature Controlled DC Fan

 ## Abstract
 
 The project will display the arrangement, layout, development, control and analysis of an automatic switching speed electric fan. The speed of the fan 
 naturally switches as indicated from sensors by environment temperature changes. This venture of a smart electric fan
 can be termed as "clever innovation". The microcontroller base programmed fan substructure introduced in this
 project is required to satisfy the necessity of advances "tomorrow will be better than today".
 
 ## Requirements
 
 ## HIGH LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- | 
|HLR01|Shall be able to run the motor according to threshold temperature |technical|  
|HLR02|Shall able to sense the temperature efficiently and precisely|technical|
|HLR03|Shall be able to display temperature|technical|
  

## LOW LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- |
|LLR01|Shall have power supply and L239D motor driver|technical|  
|LLR02|Shall have LM35, ADC|technical|
|LLR03|Shall have LCD display to show the current temperature |technical|

## Application

 1. This can be used in home applications.
 2. The circuit can be used in CPU to reduce the heat.

## SDLC

a) Sensors:

**LM35** - LM35 is a device which converts the physical signal into electrical signal which is also why this is known as the transducer.

**ADC0804** - ADC0804 is an integrated circuit which converts the input analog voltage to its equivalent digital output. (ADC0804 is an 8-bit ADC)

b) Actuators: 

**Motor drive/ FAN** - This is an external device which is the added to implement the output of the system.



### Brief about the components:

1. **Temperature sensor** : It is a device that detects and measures hotness and coolness and converts it into an electrical signal. 

    * LM35 - LM35 is a device which converts the physical signal into electrical signal which is also why this is known as the transducer.
    * ADC0804 - ADC0804 is an integrated circuit which converts the input analog voltage to its equivalent digital output. (ADC0804 is an 8-bit ADC)
    
     **These two devices are used to take the data from surrounding and then converting the analog data to digital**
     
2. **Microcontroller** : A microcontroller is a small computer on a single metal-oxide-semiconductor integrated circuit chip. A microcontroller contains one or more CPUs along with memory and programmable input/output peripherals.

    * ATmega8 microcontroller contains 8 Kb Flash system memory around 10,000 times it can be write or erased.
    * It has 512 bytes of EEPROM and it can perform write or erase operation 100,000 times.
    * It also has 1 Kb internal Static RAM.
    
3. **LCD** : This will be used to display the data. This is a type of flat panel display which uses liquid crystals in its primary form of operation.
4. **TRIAC** :  TRIAC is triggered into conduction in both directions by a gate signal like that of an SCR. TRIACs were designed to provide a means for the development of improved AC power controls.
 
5. **Motor/Fan** : This is an external device which is the added to implement the output of the system.
    
    
   
## Basic flow diagram to illustrate the working:


![dcfan1](https://user-images.githubusercontent.com/98945487/154833972-e9a8b1b7-26a5-41e6-9303-368f1e60f824.JPG)

