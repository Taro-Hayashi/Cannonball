# Cannonball カーソルパッド Build Manual ([日本語](https://github.com/Taro-Hayashi/Cannonball/blob/main/README.md))
- [Contents](#Contents)
- [Soldering](#Soldering)
- [Testing](#Testing)
- [Assembling](#Assembling)
- [Customize](#Customize)

## Contents
![](img/IMG_3856.jpg)
||Name|Quantities| |
|-|-|-|-|
|1|Main Board|1||
|2|Middle plate #1|1||
|3|Middle plate #2|1||
|4|Bottom plate|1||
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
|16|Lever Switches|2|Assembled|
|17|Rubber feet|6||

## Additional required
|Name|Quantities||
|-|-|-|
|Pro Micro (With Conthrough)|1|[Yushakobo](https://shop.yushakobo.jp/en/products/promicro-spring-pinheader)|
|Switches|9|Kailh Low Profile Switches V1/V2|
|Keycaps|9|8: 1U, 1: 2U|
|Micro-USB Cable|1|[Yushakobo](https://shop.yushakobo.jp/en/products/usb-cable-micro-b-0-8m)|

## Optional
|Name|Quantities||
|-|-|-|
|SK6812MINI-E|9|[Yushakobo](https://shop.yushakobo.jp/en/products/sk6812mini-e-10)|
|WS2812B|3|[Yushakobo](https://shop.yushakobo.jp/en/products/a0800ws-01-10)|

## Soldering
Remove protection plate, screws and spacers.  
![](img/IMG_2762.jpg)  

Install the diodes from D1 to D13.  
![](img/diode0.jpg)  
Diodes have a direction.  

Bend the legs parallel to the diode to prevent interference with the key switch later.  
![](img/diode2.jpg)  

Solder and cut the legs.  
![](img/diode3.jpg)  

Solder Tactile Switches. 
![](img/reset1.jpg)  

Solder and cut the legs.  
![](img/reset2.jpg)  

Solder Switches.  
![](img/keyswitch1.jpg)  
The two switches here may come in contact with the Pro Micro, so cut off the legs before soldering.  
![](img/keyswitch2.jpg)  
In the case of the choc V1 switch, one of the legs will interfere with the switch, so cut it short.  
![](img/keyswitch3.jpg)  

Put conthroughs. Make the top and bottom and front and back the same.  
Conthroughs are not soldered so that Pro Micro can be removed.  
![](img/promicro1.jpg)   

And put Pro Micro on conthroughs.
![](img/promicro2.jpg)   

And put Pro Micro on conthroughs.
![](img/promicro3.jpg)   

Solder rotary encoders
![](img/wheel1.jpg)  
![](img/wheel2.jpg)  
![](img/wheel3.jpg)  
![](img/rot1.jpg)
![](img/rot2.jpg)  
![](img/rot3.jpg)  


## Testing
Connect one of them to the PC with a USB cable.  
Access Remap's firmware page with Chrome or Edge.  
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware

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
![](img/bottom01.jpg)  
There will be middle spacers on the side of the key switch.  
![](img/bottom02.jpg)  

Attach short spacers on the back of the main board with short screws.  
And fit the middle plate #1.  
![](img/bottom03.jpg)  

Fasten the middle plate #2 and the back plate with long screws.  
![](img/bottom04.jpg)  
![](img/bottom05.jpg)  

Attach cover plate to the front with middle screws.  
![](img/bottom06.jpg)  

After installing the keycap, follow the same procedure as before to update the firmware for production.  
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
![](img/remap06.jpg)  

Attaching the knob and rubber feet.  
![](img/rubber.jpg)  
![](img/done.jpg)  
Thank you for your time.  

## Customize
![](img/layout.jpg)  
[Keyboard Layout Editor](http://www.keyboard-layout-editor.com/#/gists/2fe2023fd6a9318985b9c40c264c6cef)  

Access Remap.  
- Remap https://remap-keys.app/

Select the blue button on the left to proceed.  
![](img/remap1.png)  

After Drag-and-Drop the keys, press the flash button in the upper right corner.  
![](img/remap3.png)  

## Misc
Firmware
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/cannonball

JSON for Remap/VIA
right-hand [cannonball.json](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.15/cannonball.json)  
left-hand [cannonball_left.json](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.15/cannonball_left.json)  

Plates data  
[cannonball_plates.zip](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.20/cannonball_plates.zip)  

Used foostan's footprint.  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  

Used plut0nium's footprint.  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

- Yushakobo: https://shop.yushakobo.jp/en/products/2797   
- BOOTH: https://tarohayashi.booth.pm/items/3172502
