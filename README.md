# PicoKey 

I go to highschool, and teens are always around when i try to login to my mail or github or any other account, so my password can be compromised.  

To solve this, I created PicoKey, which is a hardware pass key in a very small form factor. It uses the RP2350A chip, although I wanted to use my favourite MCU, the rp2040, it was not safe as a pass key, so I used the rp2350A this time, which is much more safer and secure than the RP2350A.  

I think it can also function as a USB-HID device because it has an external button too and 16Mb of memory size.

It has USB-A in the PCB itself soo need for external connectors, however, you either need to order a 2.0mm thick PCB(expensive) or you need to order a 1.6mm PCB(pretty cheap) and make up for the 0.4mm using tape or some other method.  

### Features:
> Small form factor: 3.45cm x 1.85 cm  
> Uses the latest MCU from Raspberyy Pi, the RP2350A  
> Could Potentially have HID Compatibility  

Idea taken from ```@Rudy``` 's [RP2350 hardware key](https://github.com/Outdatedcandy92/PicoDucky)  

# How to Assemble this PCB?

It is basically a single pcb, so assembling this project means soldering on all the components.  

To solder, I would recommend buying a stencil along with the PCBs, or opting for PCBA from your PCB manufacturer, I am using [JLC](https://jlcpcb.com) for this, and I will be opting for PCBA, as this is a 2 sided board, it will be much easier for 1 side to be PCBA(bottom side) and other by hand(top side).  

The RP2350A is housed on the bottom side along with most of the components, and I have placed easy to solder components on the top, and the small pads for resistors and LED are a little bigger, which would help in soldering by hand.

# Why i chose to make this project
I chose to make this project mainly for 2 reasons:  

1. i wanted to have a secure hardware key and didn't wanna sign in using passwords in front of everyone.  

2. I wanted to try out making a 2 sided PCB(where components are on 2 sides), to learn how to make such projects and the learning curve for dual sided PCBs.  

# Images
![final pcb img](/images/8/pcb_final_3.png)  
![final cad 1](/images/8/3d_1_final_2.png)  
![final cad 2](/images/8/3d_2_final_2.png)  
![final sch img](/images/5/sch_final.png)  


# BOM

| ITEM NAME                   | ITEM PRICE | FUNCTION                 | URL                                       |
| --------------------------- | ---------- | ------------------------ | ----------------------------------------- |
| Pcb Manufacturing + stencil | 23.82      | main pcb and smt stencil | [https://jlcpcb.com](https://jlcpcb.com/) |
| PCB Components              | 21.1131    | components on the PCB    | [https://lcsc.com](https://lcsc.com/)     |
|  Total                  | 44.93      | USD                      |                                           |

# PCB Components Breakdown