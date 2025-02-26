# 3in1 WIFI Board with Screen
Update: 21 Feb 2025 by John @ Honey Honey Team

![Alt text](assets/images/Front.WithFZ.white.jpg)
![Alt text](assets/images/Front.withoutFZ.white.black.jpg)
![Alt text](assets/images/back.withoutFZ.white.black.jpg)
![Alt text](assets/images/Back.WithoutFZ%2Cwhite.black.jpg)
![Alt text](assets/images/side.withoutFZ.white.black.jpg)
![Alt text](assets/images/Top.withFZ.white.jpg)
![Alt text](assets/images/Top.WithFZ.black.jpg)
![Alt text](assets/images/antenna.bottom.jpeg)
<br/>


## What is it, and what can the board do??

The 3-in-1 board contains three chipsets: ESP32, nRF24, and CC1101. 

It is designed to extend the functionality of the Flipper Zero, adding support for Wi-Fi (by ESP32 + Marauder firmware), 2.4GHz RF (by nRF24), and expanded SubGHz coverage (by CC1101).

<br/>

## Specification of the board

- ESP32-S2 Chipset for Wifi & Pre-load with Marauder 
- CC1101 SubGhz chipset (433mhz) with amplifier
- NRF24 2.4Ghz Chipset 
- 1.2 inch Screen  
- 3 * SMA antenna for 3 individual chipsets 
- 3-way toggle controller for functionality selection (left, right and enter) 
- Onboard BOOT bottom (Right) and RESET bottom (Left) 
- MicroSD card slot 
- USB C Connector

<br/>

  
## How the board operate 

- Simply plug the board into the Flipper Zero, use the toggler to select one of the three chipsets and confirm the selection, then choose one of the relative apps on the Flipper, and you're good to go.
- The nRF24 and CC1101 chipsets do not require additional firmware to function. Most Flipper Zero firmware, including Momentum, Unleashed, and others, support them natively.
- The ESP32 requires Marauder firmware to function, and it comes pre-loaded with the firmware on the ESP32 chipset.

<br/>

## CC1101 Amplifier Explanation

The switch at the back of the board is for the SubGHz CC1101 amplifier. (The switch can be accessed by disassembling the 3D-printed case.)
- When the switch is set to **TX**, it **amplifies the transmitting signal** of the CC1101 chipset. 
- When the switch is set to **RX**, it **amplifies the receiving signal** of the CC1101 chipset. 
- Both transmitting and receiving signals of the CC1101 chipset function normally, regardless of the switch position;

<br/>

## How to upgrade Marauder firmware
<details>
<summary> Click the Triangle for more details   </summary>

To flash the Marauder onto the board, we suggest using **Google Chrome**.  

There are two buttons located near the screen: the button on the right is the Boot button, and the one on the left is the Reset button. 

1. Open the Web Flasher called < ESPWebTool > [https://esp.huhn.me/](https://esp.huhn.me/). 

2. Connect the USB-C cable to your laptop or computer. Then, while **holding the BOOT button** (on the right side of the board), plug the USB-C cable into the board. AKA, getting the board into Bootloader mode rather than starting up normally

   ![Alt text](assests/images/)  ---- **add photo of the buttom**  

4. Then, click "Connect" on the website.

![Alt text](assests/images/ESPwebtool.connect.png?raw=true)
   
4. In the prompt window, select <ESP32-S2 (COM X)> (X will be a number between 1 and 9). 

5. Open [Marauder firmware website](https://github.com/justcallmekoko/ESP32Marauder/wiki/update-firmware#using-spacehuhn-web-updater), and download the **four** related files under **Flipper Zero WiFi Dev Board**, as the 3-in-1 board uses the same chipset as the original Flipper WiFi Dev Board, as showed in the following picture. 

6. Next, load up the files into the ESPWebTool as shown in the picture. After double-checking that you've selected the correct files, click "PROGRAM."

![Alt text](assests/images/ESPwebtool.files.png?raw=true)   

7. The system should be ready to go in a few minutes.

FYI. 

- Some people might need a few attempts to get it working during the process of getting the board into Bootloader mode, aka holding the BOOT button and connecting the USB-C cable, and the web refresher recogize it. Just be patient and try a few times.
- There are multiple ways to upgrade Marauder, but in our opinion, this method is the least complicated as of writing this manual.

</details>

<br/>

## Our official shop if you would like to support us.  
1. [Our official site](https://honeyhoneylab.com/)
2. [Tindie](https://www.tindie.com/stores/honeyhoneytrading/)
3. eBay
4. ~~[ETSY Shop](https://www.etsy.com/au/shop/HoneyHoneyTrading)~~

<br/>

## Warrenty and Tech Support

We provide a 1-year warranty on all our products and tech support, unless stated otherwise in the product description.

FYI, our [Etsy](https://www.etsy.com/au/shop/HoneyHoneyTrading) shop is no longer in operation. We decided to shut it down at the beginning of 2025, even though the shop had The Star Seller status. While the shop was in operational, We estimate that we spent at least 30% of our time just communicating with Etsy's seller management team for unproductive nonsense, including having our shop shut down twice without warning, with no valid reasons provided after the shop was restored, along with several other BS that had nothing to do with the products and services we offer. 

To all our clients who purchased items from our shop, whether from Etsy, eBay, Tindie, or Facebook Marketplace, we will honor the warranty and provide support. Please feel free to email us at Support@honeyhoneylab.com. or Whatsapp 

<br/>

## Credibility
- Credit of the [web flasher](https://esp.huhn.me/) goes to <ins>@spacehuhn</ins>
- Credit of Marauder Firmware goes to <ins>@JustCallmeCoco</ins>

<br/>

## FAQ 

To be continue.

<br/>

### Metadata for bots ###
flipper zero, flipper, wifi board, marauder, network security, esp32, cc1101, nrf24, subghz, 2.4ghz, wifi, 
