# CartridgeDuino

A MSX version of the TZXDUINO.
Designed by @edu_arana | coworked with @jgilcas & @pablibiris

Based on the original design of Andrew Beer, Duncan Edwards.

This CartridgeDuino / tzxduino version has been made to act as an MSX cartridge but only to take the power +5V and GND from the MSX connector and use it on the board. Also the arduino pro mini has been replaced with a NANO to make easy to upgrade. I have used parts of my TZXDUINO RELOADED design for this.

# Works with

- TSX, CAS (MSX)

# Note

This is a work in progress, several testing must be made but it should work as is. I take no responsibiltiy for any damage to any equipment that results from the use of this board. USE AT YOUR OWN RISK!

If you like the project or want to support it, you can buy me a beer or a KO-FI :) 
[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/H2H51MPWG)

# Images

<img src="https://github.com/arananet/CartridgeDuino/blob/master/images/top3.png?raw=true" width="700">

# Instructions
 
1. Download the official TzxDuino code from http://arduitapemarkii.blogspot.com.es/2017/06/tzxduino-17.html 
2. Set the display hardware address on the TZXDuino_V1.7b.ino depending on what kind of display have. If does not work, use a i2c scanner in order to get the exact hardware address from the display.
3. Plug the Arduino Nano on the computer and use the Arduino IDE to upload the code into it.
4. Plug an MicroSD card with all the files and enjoy the power of the TzxDuino!

# Updates
12/11/2019: Updated license stuff (I usually not do this but I must start it with this).
01/08/2018 Fixed jacks positions, changed oled 128x64 for 128x32.
31/07/2018 Initial release.

# Bill of materials

| Part          | Value                   | Package                        |
| ------------- | ----------------------- | ------------------------------ | 
| M1            | ARDUINO NANO            | PCB                            |
| IC1           | 4050D                   | SO16                           |
| JP1           | OLED SCREEN CONNECTOR   | 1X04_ROUND                     |
| POWER         | SMD 0805 LED            | CHIP-LED0805                   |
| ACT           | SMD 0805 LED            | CHIP-LED0805                   |
| R2 (FOR LED)  | 330/560/1K              | R0805                          |
| R3 (FOR LED)  | 330/560/1K              | R0805                          |
| PLAY          | PUSH BUTTON             | B3F-31XX                       |
| DOWN          | PUSH BUTTON             | B3F-31XX                       |
| ROOT          | PUSH BUTTON             | B3F-31XX                       |
| STOP          | PUSH BUTTON             | B3F-31XX                       |
| UP            | PUSH BUTTON             | B3F-31XX                       |
| SD1           | MicroSD socket          | TF-PULL                        |
| X1            | STEREOJACK 3.5mm        | STX3100                        |
| X2            | STEREOJACK 2.5mm        | PJ-204B                        |


This is the arduino used in the board.

https://es.aliexpress.com/store/product/Freeshipping-Nano-3-0-controller-compatible-for-arduino-nano-CH340-USB-driver-NO-CABLE/731260_32341832857.html?spm=a219c.search0104.3.1.142e11c3RzMxTN&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_10547_10342_10343_10340_10548_10341_10696_5011015_10084_5010915_10083_10618_10307_10820_10301_10821_10303_10869_10868_10059_100031_10103_10624_10623_10622_10621_10620,searchweb201603_45,ppcSwitch_5&algo_expid=640ed1a6-ad12-4a2c-ab1d-79a6ba737643-0&algo_pvid=640ed1a6-ad12-4a2c-ab1d-79a6ba737643&priceBeautifyAB=0

# License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0
International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
