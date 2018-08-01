# CartridgeDuino
A MSX version of the TZXDUINO made by @edu_arana and coworked with @jgilcas.

Based on the original design of Andrew Beer, Duncan Edwards.

This CartridgeDuino / tzxduino version has been made to act as an MSX cartridge but only to take the power +5V and GND from the MSX connector and use it on the board. Also the arduino pro mini has been replaced with a NANO to make easy to upgrade. I have used parts of my TZXDUINO RELOADED design for this.

# Works with

- TSX, CAS (MSX)

# Note

This is a work in progress, several testing must be made but it should work as is. I take no responsibiltiy for any damage to any equipment that results from the use of this board. USE AT YOUR OWN RISK!

If you like the project, buy me a beer or a Mercedes Benz SLR whatever you want :) - info@arananet.net

# Images

<img src="https://github.com/arananet/CartridgeDuino/blob/master/images/top3.png?raw=true" width="700">

# Instructions
 
1. Download the official TzxDuino code from http://arduitapemarkii.blogspot.com.es/2017/06/tzxduino-17.html 
2. Set the display hardware address on the TZXDuino_V1.7b.ino depending on what kind of display have. If does not work, use a i2c scanner in order to get the exact hardware address from the display.
3. Plug the Arduino Nano on the computer and use the Arduino IDE to upload the code into it.
4. Plug an MicroSD card with all the files and enjoy the power of the TzxDuino!

# Updates
01/08/2018 Fixed jacks positions, changed oled 128x64 for 128x32.
31/07/2018 Initial release.

# Bill of materials

| Part          | Value                   | Package                        |
| ------------- | ----------------------- | ------------------------------ | 
| C1            | 10uf/22uf               | C0805K                         |
| C2            | 10uf/22uf               | C0805K                         |
| C3            | 0.22uF                  | C0805K                         |
| C4            | 10uf                    | C0805K                         |
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
