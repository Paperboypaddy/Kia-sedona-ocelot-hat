# Kia Sedona 2004 Ocelot Hat
The idea of this Ocelot V2 Hat design is to control the stock cruise control system in the car currently as well as adding a K Line Lin Bus tranciever to act like a ELM327 to capture car speed and other stats for openpilot.

<img src="https://github.com/Paperboypaddy/Kia-sedona-ocelot-hat/blob/main/Images/Hat_Board_Top.jpg" width="600">
<img src="https://github.com/Paperboypaddy/Kia-sedona-ocelot-hat/blob/main/Images/Hat_Board_Bottom.jpg" width="600">
Im using a MC33660BEFR2 chip to interface with Lin Bus K-Line over serial USART. USART isconnected to PB10 (TX) and PC5 (RX) on the Ocelot, along with Enable connected to PB1.

As for the cruise control switches and mosfets, my stock cruise control system is using 12v signals for the buttons. The series of mosfets are connected to PC10 (CCSET_INPUT) and PC11 (CCRES_INPUT). And the Stock Switches are connected to 3.3V and PC12 (CCSET_SW) and PD2 (CCRES_SW). 

I've also added a RGB status LED in place where the Black Panda would have had one.
<img src="https://github.com/Paperboypaddy/Kia-sedona-ocelot-hat/blob/main/Images/Hat_Board_Sch.png" width="600">
<img src="https://github.com/Paperboypaddy/Kia-sedona-ocelot-hat/blob/main/Images/Hat_Board.jpg" width="600">
