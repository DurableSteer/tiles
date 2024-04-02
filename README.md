![single_tile](https://github.com/DurableSteer/tiles/assets/140595465/330805dd-f951-40a7-80c1-63ac52a086ab) ![two_tiles](https://github.com/DurableSteer/tiles/assets/140595465/c17181ee-2853-4c1f-89c7-32e10b81e5ae)

(excuse my crappy phone camera)

# tiles
Gif tiles are small modular displays that can play animated gifs. The tiles share a common usb power source and connect magnetically so they can be rearranged as one likes and multiple tiles only use one power cable. The tiles use an esp8266 module and gifs are uploaded easily from any computer in the WiFi network via a basic GUI i called tileman.

This is going to cover the software side of this project. If you are looking for the hardware side and building instructions they can be found at [insert link] .

## dependencies
The tileman script uses PyQt6, and ftplib. 
It also uses my convert.py script.

The convert script uses Pillow, and the colorthief module.
All of those libraries can be installed via pip easily.

Furthermore the convert script uses gifscicle by kohler (https://github.com/kohler/gifsicle) which can be downloaded from https://www.lcdf.org/gifsicle/ . 
The convert script requires the gifscicle.exe to be in the same working directory as convert.py!

The gif_tile sketch uses the following libraries:
- AnimatedGIF by bitbank2 (https://github.com/bitbank2/AnimatedGIF)
- WiFiManager by tzapu (https://github.com/tzapu/WiFiManager)
- SimpleFTPServer by xreef (https://github.com/xreef/SimpleFTPServer)
- TFT_eSPI by Bodmer (https://github.com/Bodmer/TFT_eSPI)
These libraries can be simply installed from the library manager in the arduino ide.
