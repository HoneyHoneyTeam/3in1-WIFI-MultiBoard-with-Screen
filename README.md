# 3in1-WIFI-Board-with-Screen
Update: 21 Feb 2025 by John @ Honey Honey Team

## What is 3in1 stands for.  

3-in-1 means there are three chipsets on a single board: ESP32, nRF24, and CC1101.

## What does 3in1 Wifi Board use for.

The board is designed for the Flipper Zero and extending Flipper functionality, including Wi-Fi, RF 2.4GHz support, and an expanded SubGHz coverage


## Specification

- ESP32-S2 Chipset for Wifi & Pre-load with Marauder firmware 
- CC1101 SubGhz chipset (433mhz) with amplifier
- NRF24 2.4Ghz Chipset 
- 1.2 inch Screen  
- 3 * SMA antenna for 3 individual chipsets 
- Toggle controller for functionality selection 
- Onboard BOOT bottom (Right) and RESET bottom (Left) 
- MicroSD card slot 
- USB C Connector
  
## How to operate 

- Simply plug in the board to the Flipper Zero, use the toggle to select one of the three chipsets, choose the app via the Flipper, and you’re good to go.

## CC1101 Amplifier Explanation

The switch at the back of the board is for the SubGHz CC1101 amplifier. 
- When the switch is set to **TX**, it **amplifies the transmitting signal** of the Sub chipset. 
- When the switch is set to **RX**, it **amplifies the receiving signal** of the CC1101 chipset. 
- Both transmitting and receiving signals of the chipset function normally, regardless of the switch position;
  
## How to upgrade Marauder firmware

To flash the Marauder onto the board, we suggest using **Google Chrome** or **Microsoft Edge**.  

There are two buttons located near the screen: the button on the right is the Boot button, and the one on the left is the Reset button. 

1. Open the Web Flasher called < ESPWebTool > by following this link: [https://esp.huhn.me/](https://esp.huhn.me/). 
 

2. Connect the USB-C cable to your laptop or computer. Then, while holding the Boot button (on the right side of the board), plug the USB-C cable into the board. AKA, getting the board into Bootloader mode rather than starting up normally

3. Then, click "Connect" on the website. 

4. In the prompt window, select <ESP32-S2 (COM X)> (X will be a number between 1 and 9). 

5. Open [Marauder firmware website](https://github.com/justcallmekoko/ESP32Marauder/wiki/update-firmware#using-spacehuhn-web-updater), and download the **four** related files under **Flipper Zero WiFi Dev Board**, as the 3-in-1 board uses the same chipset as the original Flipper WiFi Dev Board.

6. Next, select the files as shown in the picture. After double-checking that you've selected the correct files, click "PROGRAM."

7. The system should be ready to go in a few minutes.

FYI. Some people might need a few attempts to get it working during the process of getting the board into Bootloader mode, aka holding the BOOT button and connecting the USB-C cable, and the web refresher recogize it. Just be patient and try a few times.

## Q & A
#
#
# credibility
- Credit of the [web flasher](https://esp.huhn.me/) goes to @spacehuhn
- Credit of Marauder Firmware goes to @JustCallmeCoco
