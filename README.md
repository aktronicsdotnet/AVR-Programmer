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
This is the easier version, all you need to do is to solder Arduino pin headers (D0 to D13 and power headers) and the ZIF socket. Bam... you are done and now you can upload the AVR as ISP sketch in Arduino ide, plug the shield and use it to program different type of AVR MCUs. Optionally you can populate the R1 and R2 with their respected LEDS to be able to visually see the progress of programming your MCUs and perhaps populate the external crystal socket, C5 and C6 to use external clocks with your MCUs.
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
What can I do with AAVR-Programmer as standalone USBASP?
</b><br>
Well in this case you can use the MicroUSB port to burn the bootloader or program any AVR MCUs that are supported by USBASP. You can directly plug it on Arduino UNO to burn the bootloader or program them, in this case close the Hardware Reset jumper or you can use this board to program other arduino boards with the 6 pin ISP connector with the standard pinout. 
<br><br>
