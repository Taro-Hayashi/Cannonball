# Cannonball カーソルパッド Build Manual ([日本語](https://github.com/Taro-Hayashi/Cannonball/blob/main/README.md))
- [Contents](#Contents)
- [Soldering](#Soldering)
- [Testing](#Testing)
- [Assembling](#Assembling)
- [Customise](#Customise)

## Contents
![](img/IMG_1757.jpeg) 
||Name|Quantities| |
|-|-|-|-|
|1|Main board|1||
|2|Bottom plate|1||
|3|Middle plate #1|1||
|4|Middle plate #2|1||
|5|Cover plate|1||
|6|Short screws|4|3mm|
|7|Middle screws|2|4mm|
|8|Long screws|6|6mm|
|9|Short spacers|6|3mm|
|10|Middle spacers|2|4mm|
|11|Diodes|13|1N4148|
|12|Tactile Switches|1||
|13|Dial Rotary Encoder|1|EC11|
|14|Knob|1||
|15|Wheel Rotary Encoders|2|EVQWGD001|
|16|Rubber feet|6||
|17|Pro Micro|1||

## Additional required
|Name|Quantities||
|-|-|-|
|Switches|9|Kailh Low Profile Switches V1/V2|
|Keycaps|9|8: 1U, 1: 2U|
|USB Cable|1||

## Optional
|Name|Quantities|||
|-|-|-|-|
|SK6812MINI-E|9|[Usage](led_EN.md)||
|WS2812B|3||

## Soldering
Install the diodes from D1 to D13.  
![](img/IMG_1794.jpg)  
Diodes have a direction.  

Bend the legs parallel to the diode to prevent interference with the key switch later.  
![](img/IMG_1798.jpeg) 

Solder and cut the legs.  
![](img/IMG_1800.jpeg)  

Solder Tactile Switches.  
![](img/IMG_1805.jpeg) 
If you want to remove the flux from the surface, now is the time.  
![](img/IMG_1821.jpeg) 

Solder Switches.  
![](img/IMG_1852.jpeg)  
The two switches here may come in contact with the Pro Micro, so cut off the legs before soldering.  
![](img/IMG_1859.jpeg)  
In the case of the choc V1 switch, one of the legs will interfere with the switch, so cut it short.  
![](img/IMG_1145.jpg)  
![](img/IMG_1148.jpg)  

Solder Pro Micro.  
![](img/IMG_1874.jpeg)  
![](img/IMG_1878.jpeg)  

Solder rotary encoders.  
![](img/IMG_1887.jpeg)  
![](img/IMG_1895.jpeg)   
![](img/IMG_1901.jpeg)   
![](img/IMG_1904.jpeg)  
![](img/IMG_1905.jpeg)  

## Testing
Connect one of them to the PC with a USB cable.  
Access Remap's firmware page with Chrome or Edge.  
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

Flash the Test firmware.  
![](img/remap02.jpg)  
![](img/remap03.jpg)  

Push the tactile switch.  
![](img/remap04.jpg) 
![](img/remap05.jpg) 

Make sure all switches are responsive.  
If there are no problems, soldering is finished.  

## Assembling
Disconnect the USB cable. 

Attach the short and middle spacers to the red circle.  
![](img/IMG_1928.jpeg)   
There will be middle spacers on the side of the key switch.  
![](img/IMG_1923.jpeg)  

Fasten the middle plate #2 and the back plate with long screws.  
![](img/IMG_1937.jpeg)  
![](img/IMG_1940.jpeg)  

Attach cover plate to the front with middle screws.  
![](img/IMG_1948.jpeg)  

Attaching the knob and rubber feet.  
![](img/IMG_1951.jpeg)  
Thank you for your time.  
After installing the keycap, follow the same procedure as before to update the firmware for production.  
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
![](img/remap06.jpg)  
  
### Firmware Code
- https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/cannonball

### Plates data  
- [cannonball_plates.zip](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.31/cannonball_plates.zip)  

### Misc
Used foostan's footprint.  
- https://github.com/foostan/kbd/  
- https://github.com/foostan/kbd/blob/master/LICENSE  

Used plut0nium's footprint.  
- https://github.com/plut0nium/0xLib  
- https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

- Yushakobo: https://shop.yushakobo.jp/en/products/2797   
- BOOTH: https://tarohayashi.booth.pm/items/3172502
