# Complex Embedded System Case Study - Temperature Controlled DC Fan

## Temperature controlled DC fan from embedded system point of view:

A Temperature Controlled DC Fan is a system which automatically turns on a DC Fan when the surrounding temperature rises above a certain limit.


Basic flow diagram to illustrate the working:
![dcfan1](https://user-images.githubusercontent.com/98945487/154833972-e9a8b1b7-26a5-41e6-9303-368f1e60f824.JPG)


## SDLC

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
 
    
    
    
## HIGH LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- | 
|HLR01|User should be able to view the correct output on LCD|non-technical|  
|HLR02|User should able to supply power manually|technical|
|HLR03|The system sould able perform the given operation successfully|technical|
|HLR04|The system should provide correct result|technical|   

## LOW LEVEL REQUIREMENTS
| ID | Description | Category | 
| ----- | ----- | ------- |
|LLR01|Power Switch|technical|  
|LLR02|LCD Display|technical|
|LLR03|Temperature Sensor|technical|
|LLR04|TRIAC|technical|
|LLR05|FAN|technical|
|LLR06|MICROCONTROLLER|technical|
 
