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

### Note: There are a few resistors and capacitors, which had very high minimum order quantity(MOQ), about 50 pieces so i had to forcefully include those, which i will be utilising in my next highway projects. And tbh the prices were very less(about $0.02 per piece) so i think it is alright

### if DNO is yes, i am not ordering the respective parts and thus i have not included the cost in BOM.


| Id | Designator                                             | Designation   | MPN                   | Footprint                       | DNO - Do not order | MOQ | Price  | Quantity | Amount | Supplier link                                                                                                                                  |
| -- | ------------------------------------------------------ | ------------- | --------------------- | ------------------------------- | ------------------ | --- | ------ | -------- | ------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | C1, C2, C3                                             | 4.7u          | GRM155R61C475KE15D    | 402                             | No                 | Yes | 0.057  | 10       | 0.57   | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Murata-Electronics-GRM155R61C475KE15D_C426094.html                  |
| 2  | C10, C11, C12, C13, C14, C15, C16, C17, C6, C7, C8, C9 | 100n          | GRM155R61H104JE14D    | 402                             | Yes                | \-  | 0      | 36       | 0      | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Murata-Electronics-GRM155R61H104JE14D_C426067.html                  |
| 3  | C18, C19                                               | 15p           | GJM1555C1H150FB01D    | 402                             | Yes                | \-  | 0      | 6        | 0      | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Murata-Electronics-GJM1555C1H150FB01D_C441742.html                  |
| 4  | C4, C5                                                 | 10u           | CL21A106KBVNNNE       | 805                             | No                 | Yes | 0.046  | 5        | 0.23   | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Samsung-Electro-Mechanics-CL21A106KBYQNNE_C2932476.html             |
| 5  | D1                                                     | LED           | 19-213-GHC-YR1S1N-3T  | 402                             | Yes                | \-  | 0      | 3        | 0      | https://www.lcsc.com/product-detail/LED-Indication-Discrete_Everlight-Elec-16-213-GHC-YR1S1N-3T_C2980183.html?s_z=n_LED                        |
| 6  | D2                                                     | ESDS314DBVR   | ESD5314DBVR           | 402                             | No                 | Yes | 0.212  | 5        | 1.06   | https://lcsc.com/product-detail/ESD-and-Surge-Protection-TVS-ESD_TI-ESDS314DBVR_C1847859.html                                                  |
| 7  | J1                                                     | USB_A         | \-                    | USBPCB                          | On PCB             | \-  | \-     | \-       | \-     | \-                                                                                                                                             |
| 8  | L1                                                     | 3.3u          | A201610S3R3-101-T     | 806                             | No                 | Yes | 0.2592 | 5        | 1.3    | https://lcsc.com/product-detail/Power-Inductors_Abracon-LLC-AOTA-B201610S3R3-101-T_C42411119.html                                              |
| 9  | R1                                                     | 33            | RT0402BRD0733RL       | 402                             | No                 | Yes | 0.0198 | 50       | 0.99   | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RT0402BRD0733RL_C852729.html                                                 |
| 10 | R2, R5, R6, R7                                         | 1k            | CRCW040210K0FKEDHP    | 402                             | No                 | Yes | 0.023  | 20       | 0.46   | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_Vishay-Intertech-CRCW04021K00FKEDHP_C313354.html                                   |
| 11 | R3, R4                                                 | 27            | ERJ2GEJ270X           | 402                             | Yes                | \-  | 0      | 6        | 0      | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_PANASONIC-ERJ2GEJ270X_C278580.html                                                 |
| 12 | SW1, SW2                                               | SW_Push       | K-PTS810SJMS205MTLFSG | SW_SPST_PTS810                  | No                 | No  | 0.6    | 6        | 3.6    | https://lcsc.com/product-detail/Tactile-Switches_C-K-PTS810SJM250SMTRLFS_C116501.html                                                          |
| 13 | U1                                                     | RP2350A-QFN60 | RPi2350               | QFN-60                          | No                 | No  | 1.514  | 3        | 4.542  | https://www.silverlineelectronics.in/collections/the-raspberry-pi/products/rp2350a-raspberry-pi-microcontroller-chip-in-stock-silverline-india |
| 14 | U2                                                     | AMS1117S-3.3  | AMS1117-3.3           | SOT-89-3                        | No                 | Yes | 0.1    | 5        | 0.5    | https://lcsc.com/product-detail/Voltage-Regulators-Linear-Low-Drop-Out-LDO-Regulators_JSMSEMI-AMS1117S-3-3_C917152.html                        |
| 15 | U3                                                     | W25Q128JVS    | W25Q128JVSIM          | SOIC-8_5.3x5.3mm_P1.27mm        | Yes                | \-  | 0      | 3        | 0      | https://lcsc.com/product-detail/NOR-FLASH_Winbond-Elec-W25Q128JVSIM_C2613930.html                                                              |
| 16 | Y1                                                     | Crystal_GND24 | ABM8-27-T3            | Crystal_SMD_3225-4Pin_3.2x2.5mm | No                 | No  | 0.3737 | 3        | 1.1211 | https://www.lcsc.com/product-detail/Crystals_Abracon-LLC-ABM8-272-T3_C20625731.html?s_z=n_abm8                                                 |
|    |                                                        | Shipping      | 3.74                  |                                 |                    |     |        |          |        |                                                                                                                                                |
|    |                                                        | Handling fee  | 3                     |                                 |                    |     |        |          |        |                                                                                                                                                |
|    |                                                        | Total         | 21.1131               | USD                             |                    |     |        |          |        |                                                                                                                                                |