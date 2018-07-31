# CartridgeDuino
A MSX version of the TZXDUINO made by @edu_arana and coworked with @jgilcas.

Based on the original design of Andrew Beer, Duncan Edwards.

This CartridgeDuino / tzxduino version has been made to act as an MSX cartridge but only to take the power +5V and GND from the MSX connector and use it on the board. Also the arduino pro mini has been replaced with a NANO to make easy to upgrade.

# Works with

- TSX, CAS (MSX)

# Note

This is a work in progress, several testing must be made but it should work as is. I take no responsibiltiy for any damage to any equipment that results from the use of this board. USE AT YOUR OWN RISK!

If you like the project, buy me a beer or a Mercedes Benz SLR whatever you want :) - info@arananet.net

# Audio Amp

Since is not very clear if there is necessary a output amp, I have added a little DPDT, one position switch to bypass or enable the D9 signal to the AMP LM386. The other position will connect the D9 signal directly to the 3.5mm jack. 

# Images

<img src="https://github.com/arananet/Cartridge/blob/master/images/top.png?raw=true" width="700">

# Instructions
 
1. Download the official TzxDuino code from http://arduitapemarkii.blogspot.com.es/2017/06/tzxduino-17.html 
2. Set the display hardware address on the TZXDuino_V1.7b.ino depending on what kind of display have. If does not work, use a i2c scanner in order to get the exact hardware address from the display.
3. Plug the Arduino Nano on the computer and use the Arduino IDE to upload the code into it.
4. Plug an MicroSD card with all the files and enjoy the power of the TzxDuino!

# Updates

31/07/2018 Initial release.

# Bill of materials

| Part          | Value                   | Package                        |
| ------------- | ----------------------- | ------------------------------ | 
| C1            | 10uf/22uf               | C0805K                         |
| C2            | 10uf/22uf               | C0805K                         |
| C3            | 0.22uF                  | C0805K                         |
| C4            | 10uf                    | C0805K                         |
| C5            | 220uf (ECA-0JM221)      | CPOL-EUE1.8-4 (only with amp)  |
| M1            | ARDUINO NANO            | PCB                            |
| IC1           | 4050D                   | SO16                           |
| IC4           | LM386M-1                | SO08 (only if amp required)    |
| TTL           | PINHD_1X04              | 1X04                           |
| JP1           | OLED SCREEN CONNECTOR   | 1X04_ROUND                     |
| POWER         | SMD 0805 LED            | CHIP-LED0805                   |
| ACT           | SMD 0805 LED            | CHIP-LED0805                   |
| R1            | 10K TrimPotentiometer   | RTRIM3103   (only with amp)    |
| R2 (FOR LED)  | 330/560/1K              | R0805                          |
| R3 (FOR LED)  | 330/560/1K              | R0805                          |
| R4            | 10K                     | R0805 (only with amp)          |
| R5            | 10K                     | R0805 (only with amp)          |
| PLAY          | PUSH BUTTON             | B3F-31XX                       |
| DOWN          | PUSH BUTTON             | B3F-31XX                       |
| ROOT          | PUSH BUTTON             | B3F-31XX                       |
| STOP          | PUSH BUTTON             | B3F-31XX                       |
| UP            | PUSH BUTTON             | B3F-31XX                       |
| SD1           | MicroSD socket          | TF-PULL                        |
| X1            | STEREOJACK 3.5mm        | STX3100                        |
| X2            | STEREOJACK 2.5mm        | PJ-204B                        |
| S1            | DPDT Switch             | AYZ0202                        |

This is the arduino used in the board.

https://es.aliexpress.com/store/product/Freeshipping-Nano-3-0-controller-compatible-for-arduino-nano-CH340-USB-driver-NO-CABLE/731260_32341832857.html?spm=a219c.search0104.3.1.142e11c3RzMxTN&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_10547_10342_10343_10340_10548_10341_10696_5011015_10084_5010915_10083_10618_10307_10820_10301_10821_10303_10869_10868_10059_100031_10103_10624_10623_10622_10621_10620,searchweb201603_45,ppcSwitch_5&algo_expid=640ed1a6-ad12-4a2c-ab1d-79a6ba737643-0&algo_pvid=640ed1a6-ad12-4a2c-ab1d-79a6ba737643&priceBeautifyAB=0

This are the DPDT switches that are maybe compatible with the footprint:

https://es.aliexpress.com/store/product/70pcs-On-Off-On-6-Pin-DPDT-Vertical-Mini-SMD-SMT-Slide-Power-Switch-7x6x4mm/1178755_1953364266.html?spm=a219c.search0104.3.146.287176b1h1eqtT&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_5722813_10151_10344_10068_10342_5722613_10547_10343_5722913_10340_10341_10548_10698_10697_10696_10084_10083_5722713_10618_10307_10301_10303_5711213_10059_10184_308_100031_10103_441_10624_10623_10622_10621_10620_5722513_5711313,searchweb201603_15,ppcSwitch_5&algo_expid=6e95ecf1-40f5-4b5b-8649-c467855a15c0-22&algo_pvid=6e95ecf1-40f5-4b5b-8649-c467855a15c0&transAbTest=ae803_1&priceBeautifyAB=0
