<b>
AVR Programmer based on USBASP that can be used as a Arduino shield or standalone
</b>
<br><br>
<a href="https://raw.githubusercontent.com/skopusdotorg/AVR-Programmer/main/Images/AVR-Programmer-3d-view.jpg"><img alt="" src="https://raw.githubusercontent.com/skopusdotorg/AVR-Programmer/main/Images/AVR-Programmer-3d-view.jpg" style="width: 800px; height: 533px;" /></a>
<br><br>

<b>
What is AVR-Programmer?
</b><br>
Everyone knows that you can use Arduino UNO as a programmer for other AVR MCUs that are supported by Arduino IDE and I'm sure at some point you have heard about USBASP if you have worked with Arduino and AVR MCUs... AVR-Programmer is a combination of these two things and can be used as both of them depending on how you assemble it.
<br><br>

<b>
How to use AVR-Programmer as a shield for Arduino UNO?
</b><br>
This is the easier version; all you need to do is to solder Arduino pin headers (D0 to D13 and power headers) and the ZIF socket. Bam... you are done and now you can upload the AVR as ISP sketch in Arduino ide, plug the shield and use it to program different type of AVR MCUs. Optionally you can populate the R1 and R2 with their respected LEDS to be able to visually see the progress of programming your MCUs and perhaps populate the external crystal socket, C5 and C6 to use external clocks with your MCUs.
<br><br>

<b>
What can I do with AVR-Programmer as a shield for Arduino UNO?
</b><br>
Well together with an Arduino Uno you can burn the bootloader or even program any AVR MCUs that are supported by Arduino IDE. (Officially or with addon packages)
<br><br>

<b>
How to use AVR-Programmer as standalone USBASP?
</b><br>
To my understanding you need to have one AVR programmer or at least an Arduino UNO to be able to programmer the ATMega8 or ATMega88 on the board as a USBASP first. If you have access to a AVR programmer you can use the 6 pin ISP header on the board to program the main MCU, in this case you can skip the Arduino headers completely but if you want to use an Arduino Uno you will need those headers so you will probably need to solder the whole board. Close the Self Programming jumper when you are programming the on board ATMega MCU, this jumper will connect the U1 RST pin to the rest of Reset pins on the board to be able to put 1 in programming mode just when we need it.
<br><br>

<b>
What can I do with AVR-Programmer as standalone USBASP?
</b><br>
Well in this case you can use the Micro USB port to burn the bootloader or program any AVR MCUs that are supported by USBASP. You can directly plug it on Arduino UNO to burn the bootloader or program them, in this case close the Hardware Reset jumper or you can use this board to program other Arduino boards with the 6 pin ISP connector with the standard pinout. 
<br><br>

<b>
What are those jumpers for?
</b><br>
I think it's really self explanatory but there are 3 jumpers on this board. One is called "Self Programming" this jumper is used to program the on board MCU and its job is to connect U1 RST pin to the rest of RESET pins. Another one is called "Slow SCK" this is used to slow down the clock of SCK pin and the last one is called "Hardware Reset" this is used to connect Arduino UNO's RST Pin to the rest of RESET pins to be able to put Arduino UNO boards into programming mode.
<br><br>

<b>
How can I use this?
</b><br>
First you need to send the Gerber files from Gerber X2 folder to your fav PCB manufacturer and wait until they make the PCB for you and the you need to buy the necessary components according to the bill of material and when everything arrived careful solder them to the PCB and use it.
<br><br>

<b>
For more advanced users...
</b><br>
For more advanced users, I've left the original design so you can change anything you want. This board was designed by Altium Designer V20.
<br><br>

<b>
How can you find me?
</b><br>
I will leave my Instagram on this GitHub just in case you needed to contact me for any reason... Instagram @ skopusdotorg
<br><br>
