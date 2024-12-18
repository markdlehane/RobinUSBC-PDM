# USB-C data and power supply.

## An adaptor that allows connection from a usb power supply or laptop.
![RDSPB5331A-Circuit](https://github.com/user-attachments/assets/09436adc-0473-4d4b-b9ef-d584f81ba726)

It's available as a kit or a premade module on [Tindie](https://www.tindie.com/products/36667/).

This adaptor provides 5v & 3.3v @1A from a USB-C connector. It also provides USB D+ and D- pins so that it can be used with a laptop or computer to provide power and data. I developed this board with the assistance of the wonderful people at [PCBWay](https://www.pcbway.com/) who enabled me to take my early design and turn it into a module that I use in every project I make now.  It's a huge time saver and makes the process of connecting my development boards to a laptop, very simple.

![RDSPB5331A](https://github.com/user-attachments/assets/88a30690-3d22-49f7-a756-ffa419a5ecbb)

## Why did you make it?

I designed this module because I was tired of the standard breadboard power supplies that simply provide 5v or 3.3v from a barrel jack. The old style supplies were limited because, even if I use USB as a supply, I didn't have a data connection. 

## What makes it special?

This module is easy to use on a breadboard, can be integrated directly into a PCB project with a jumper and provides a data pathway to your embedded device. There is a transient voltage suppression device on the board to give added project from voltage spikes as the cable is connected.

## Module design

I designed this board because I have been developing project with ESP32S3 modules. These made a USB data connection immediately available, like many other alternatives, and I wanted to simplify my prototyping and development process through simplification. 

The module is supplied with an [AZ1117I](https://www.diodes.com/assets/Datasheets/AZ1117I.pdf) 3.3v LDO and the 5v is provided directly by the USB-C connection (which uses 2 5k1 1% resistors to negotiate the voltage). There is an LED on the board to indicate that 5v power is connected by this can be disconnected through a solder bridge so that it can be disabled when power must be stricly controlled.

![RobinUSBC-back-PSM](https://github.com/user-attachments/assets/f5d9463f-d933-4f49-b529-2e7d4e02d808)
![RobinUSBC-Front-PSM](https://github.com/user-attachments/assets/309420cb-ff74-473e-9321-7d02b272f1d1)
