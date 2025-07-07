# PicoKey
I go to highschool, and teens are always around when i try to login to my mail or github or any other account, so my password can be compromised.  

To solve this, i created PicoKey, which is a hardware pass key in a very small form factor. It uses the RP2350A chip, although i wanted to use my favourite MCU, the rp2040, it was not safe as a pass key, so i used the rp2350A this time, which is much more safer and secure than the rp2350A.  
I think it can also function as a USB-HID device because it has an external button too and 16Mb of memory size.

It has USB-A in the PCB itself soo need for external connectors, however, you either need to order a 2.0mm thick PCB(expensive) or you need to order a 1.6mm PCB(pretty cheap) and make up for the 0.4mm using tape or some other method.  

### Features:
> Small form factor: 3.45cm x 1.85 cm  
> Uses the latest MCU from Raspberyy Pi, the RP2350A  
> Could Potentially have HID Compatibility  

Idea taken from ```@Rudy``` 's [RP2350 hardware key](https://github.com/Outdatedcandy92/PicoDucky)  