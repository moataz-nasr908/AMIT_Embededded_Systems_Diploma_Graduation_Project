# AMIT_Embededded_Systems_Diploma_Graduation_Project 

AMIT  Graduation Project: Electric-Water-Heater





Description :

An Electric Water Heater using AVR ATmega32 chip. It consists of a lot of modules such as ADC, EEPROM, 7 Segment, Push Buttons, Leds, Interrupts and TIMERs. The heater uses the EEPROM to save the latest desired temperature the user modified.



The Controller follows the following procedure:

It has the ON/OFF Button that is attached to an external interrupt, that switches between ON and OFF states. In the OFF state everything is OFF and the desired temperature is saved in the EEPROM and the microcontroller is in sleep mode. In the ON state, the microcontroller senses the actual temperature using the internal ADC and temperature sensor (LM35) and save it to an array. The array consists of the last 10 readings that are used to make the decision of turning the heater/cooler on and off depending on their average. The UP and DOWN buttons are used to switch from the ON state to the SETTINGS state, where the user can modify desired temperature. Ff the user didn't click the UP or DOWN buttons for five seconds, it turns back to the ON state, and the chosen temperature is saved in the EEPROM once again.
The indication led is to know which element (Heater or Cooler) is working and in what state is the controller in.
