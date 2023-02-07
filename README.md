## Adafruit Feather RP2040 SCORPIO 8 Channel NeoPixel Driver PCB

<a href="http://www.adafruit.com/products/5650"><img src="assets/5650.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit Feather RP2040 SCORPIO 8 Channel NeoPixel Driver. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5650

### Description

If there is one thing Adafruit is known for, its mega-blinky-fun-rainbow-LEDs. We just love sticking NeoPixels anywhere and everywhere. When we saw the new 'PIO' peripheral on the RP2040 from Raspberry Pi, we just knew it would be perfect for driving large quantities of NeoPixels. So we created this board, the Adafruit Feather RP2040 SCORPIO, designed specifically for NeoPixel (WS2812) driving but also good for various other PIO-based projects that want to take advantage of the Feather pinout with 8 separate consecutive outputs (or inputs).

The RP2040 PIO state machine is perfect for LED driving: it can generate perfect waveforms, with up to 8 outputs concurrently, all through DMA. That means that you don't need to use any processor time to bit-bang-out the LED data. Just set up the buffer and tell the PIO peripheral to 'make it so' and it will shove that data to the 8 outputs without delay while your code can continue to read buttons, play music, run CircuitPython - whatever you like!

The SCORPIO has a clever pinout, where all the standard Feather pins are the same as the GPIO pins, plus the standard I2C, SPI and UART lines - and theres still enough pins left over to have 8 consecutive pins for PIO usage on GPIO16 through GPIO23 inclusive.

To make NeoPixel usage glitch-free there is a 3V->5V level shifter so that the output logic is 5V. If you happen to want 3V signals, you can adjust the shifter voltage with a jumper on the bottom. It's also possible to flip the direction of the level shifter to make the 8 I/O pins inputs - say for making a logic analyzer - with a directional jumper selection also on the bottom of the PCB.

The RP2040 SCORPIO also has a ton of RAM, 264KB, making it trivial to buffer huge numbers of NeoPixels…several thousand if needed. In fact there's so much RAM you can even dither the pixels to for finer brightness control, for better-looking LEDs at low brightness or for gamma correction.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
