# artnet-to-ws2812-over-arduino
a artnet to I2C convertor for controlling LEDstrips like WS2812, WS2811, SK6188,... Can be used with any software that can handle Artnet like resolume, jinx, glediator,....
/*
This example will receive multiple universes via Artnet and control a strip of ws2811 leds via 
Adafruit's NeoPixel library: https://github.com/adafruit/Adafruit_NeoPixel
This example may be copied under the terms of the MIT license, see the LICENSE file for details
*/

stuff used:
1x arduino MEGA 
1x rj 45 cable
1x ethernet shield
1x WS2812 LED strip (150 pixels in this case)
1x 5V= powersupply 300Watts (could be less or more, pending on the power and amount of LED's in the strip, i just used an old powersupply of a pc)
A PC with the software and a network connection.

when using resolume software, use following steps to get correct settings.
1) open resolume
2)go to output => advanced
3) left above corner click "+" and choose "dmx lumiverse"
4) in the right column you can click the settings symbol beside the fixture name.
5) you can change the height and width to correspond with your LED strip. (hight will be usually 1 and with is the total amouth of LED's that you have in your LED strip)
6) in the mapping window, you can drag and place your LED strip to the place you want.
7) go back to main screen and go to Arena => preferences
8) choose DMX 
9) set next settings
Device = Artnet
Lumiverse = Lumiverse 1
Subnet = 0
Universe = 1
Target IP = Broadcast

10) play some content and you will see your LED strip running 
