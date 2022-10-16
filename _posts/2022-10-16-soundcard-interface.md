---
layout: post
title: 'Soundcard Interface for Direwolf'
---
This interface is built on perfboard and meant to be mounted onto a Raspberry Pi
running direwolf. Connections to the soundcard and radio are through breakout
cables so that the interface can be configured for different radios and
soundcards.

![alt text](soundcard-interface/hat-top.jpg "component side")
![alt text](soundcard-interface/hat-bottom.jpg "wiring side")


## Screw Terminal Connections

Orient the board so that the screw terminals are on top as in the picture, terminal #1 is on left and terminal #7
is on the right.


1. PTT (from radio)
1. Gnd (from radio)
1. Gnd (from soundcard)
1. Spkr+ (from radio)
1. Mic (to sound card)
1. Left channel (from sound card)
1. Mic+ (to radio)

## Breakout Cables

### Radio Breakout Cable (Kenwood, Baofeng, etc)

3.5mm TRS Connector

- Tip
- Ring, Mic+
- Shield, PTT

2.5mm TRS Connector

- Tip, Speaker+
- Ring
- Shield, Ground

![alt text](soundcard-interface/kenwood-breakout.jpg "K1 Connector")

### Soundcard Breakout Cable

3.5mm TRRS Connector

- Tip, Left channel
- Ring, Right channel
- Ring - Ground
- Shield - Mic

![alt text](soundcard-interface/audio-breakout.jpg "TRRS Connector")

## Direwolf Configuration

- PTT is on GPIO 13
- DCD is on GPIO 4

## Schematics

- [Schematic](soundcard-interface/soundcard-interface_schem.png)
- [Fritzing](soundcard-interface/soundcard-interface.fzz)

## Resources

- [Super Simple APRS Position Reporter｜Midnight Cheese](http://midnightcheese.com/2015/12/super-simple-aprs-position-beacon/)
- [APRS – Raspberry Pi Virtual TNC – WCARES](https://wcares.org/special-interests-3/aprs/aprs-raspberry-pi-virtual-tnc/)
- [APRS RX/TX I-Gate and Digipeater for less than $100 - N1AAE](https://n1aae.com/raspberry-pi-aprs-direwolf-linux-igate-digipeater/" )
- [Soundcard interface - (including PTT) for Baofeng UV5R and other cheap handhelds](https://k0rx.com/blog/2017/11/baofeng.html)
- [Direwolf - APRS Box Documentation](http://elafargue.github.io/aprs-box/direwolf/)
- [direwolf/Successful-APRS-IGate-Operation.pdf at master · wb2osz/direwolf](https://github.com/wb2osz/direwolf/blob/master/doc/Successful-APRS-IGate-Operation.pdf)
- [Converting a CM108 USB fob for amateur radio use](https://www.marrold.co.uk/2018/04/converting-cm108-usb-fob-for-amateur.html)
- [LTV-847C Lite-On Inc. | Isolators | DigiKey](https://www.digikey.com/en/products/detail/liteon/LTV-847C/1711628)
- [A Simplified USB Sound FOB Modification](https://hamvoip.org/hamradio/usb_fob_simple_modification/)
- [How To Modify A CM108 for Allstar latest version - allstar setup.com %](https://allstarsetup.com/how-to-modify-a-cm108-for-allstar/)
- [Modifying the SYBA UAUD CM119 based USB audio adapter for use as Asterisk USB radio interface](http://www.repeater-builder.com/projects/fob/syba-small-fob.html)
- [usbfob.pdf](http://rtpdir.weebly.com/uploads/1/6/8/7/1687703/usbfob.pdf)
- [GitHub - eleccoder/raspi-pico-aprs-tnc: A modem/TNC to generate the AFSK audio tones for sending APRS messages using a Raspberry Pi Pico](https://github.com/eleccoder/raspi-pico-aprs-tnc)
- [audio - How to DIY BaoFeng radio-to-soundcard cable? - Electrical Engineering Stack Exchange](https://electronics.stackexchange.com/questions/471893/how-to-diy-baofeng-radio-to-soundcard-cable)
- [Adding PTT on USB Soundcard](https://yd0nxx.wordpress.com/2020/05/12/adding-ptt-on-usb-soundcard/)
- [ZS2EZ Soundcard Interfacing](http://www.zs2ez.co.za/Soundcard/Soundcard.htm)
- [Raspberry Pi Datasheets](https://datasheets.raspberrypi.com/)

