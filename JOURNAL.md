---
title: "PicoKey"
author: "Keyaan"
description: "A Pass Key(Like Yubikey) using the RP2350A from Raspberyy Pi!"
created_at: "2025-06-26"
---
----
# June 26 2025
Yup, I wanna make a hardware key. I was inspired by yubikey, [orpheus pico guide](http://orpheuspico.hackclub.com/docs/pico/guides/passkey), and the [RP2350 hardware key](https://github.com/Outdatedcandy92/PicoDucky) by ```@Rudy```

I might start from tomorrow.  

----
# June 27 2025

Beginning my work on PicoKey from today. The things i will try to accomplish:
> PCB Trace USB Connector  
> Use an RP2350 instead of RP2040 this time:(  
> smallest possible footprint  
> also add HID compatability
  
I wanted to use the RP2040 but it is apparently not secure enough so now i have to use the RP2350 :(

Gotta start with the schematic(i didn't)

----
# June 29 2025

Finally, my test is over today and now i can work on this PCB. so, starting with the schematic from now on.

### Time spent: about 1 hour (had to learn the rp2350 design guide)

----
# June 30 2025
I did the work yesterday but then i was ordered to chut down the laptop immediately, so i had to go, anyways, here are the pictures from yesterday:

![schematic](/images/29/schematic.png)

i didn't work on anything else.

----
# July 1 2025

I have thought of something, maybe, i can also make the device as an HID, like how ```@Rudy``` made it, so i am gonna do that probably and complete the pcb today itself.  
I think the schematic is complete, here it is:  
![schematic july 1](/images/1/schematic.png)

other than the schematic, i worked on the pcb, here is the current progress:  
![pcb july 1](/images/1/pcb.png)  

I also added an ESD protection IC, here it is:  
![esd IC](/images/1/esd.png)  


I worked more on the PCB, yeah, i realised that making a dual sided PCB is HARD, i alwasys that that i could do it easily, but no, it is hard :/
Anyways, here is the updated PCB:  
![pcb july 1](/images/1/pcb_2.png)  

### TIme Spent Today: about 1 hour and 45 mins

# July 2 2025
Yooo i am in school, gotta work on the pcb a lil bit.  
Here it the work i did:  
![pcb july 1](/images/2/pcb.png)  

i might just complete the PCB today if i get time. 
This two sided PCB is so hard to deal with 😭

### Time Spent Today: about 45 mins

# July 4 2025

I am in school againn!!! Gotta work on the PCB.
in school, i just changed the PCB side and make it round rectangular. nothing more nothing fancy, although i attracted attention of a few of my friends when doing so!

Now i am starting to work again. will update soon

yay, i worked and i think the PCB is complete. the one thing that amazes pcb makers:

![](/images/4/no_errors.png)  

And Now the PCB:  
![](/images/4/pcb.png)  
![](/images/4/pcb_poured.png)  

I still have to add some silkscreens and will do that later or tomorrow

### Time Spent Today: 1 hour 10 mins

# July 5 2025
worked on the pcb, added silkscreen layers and stuff, the final size comes to 34.5mm x 18.5mm, nice. Here is the final image of the pcb and the schematic and the 3d model:  
![final pcb img](/images/5/pcb_final.png)
![3d 1](/images/5/3d_1.png)
![3d 2](/images/5/3d_2.png)
![final sch img](/images/5/sch_final.png)


# July 7 2025:  
I will have to change the footprint of the 3.3uH inductor used for the RP2350A inbuilt regulator. Gonna do that rn.

I am done, here are the updated images:  
![final pcb img](/images/7/pcb_final_2.png)
![final cad 1](/images/7/3d_1_final.png)
![final cad 2](/images/7/3d_2_final.png)
![final sch img](/images/5/sch_final.png)

Now i am gonna try to finish writing the README tonight itself.

Oh hell nah, i forgot to label BOOTSEL AND THE BUTTON, gonna do that just now


### Time Spent Today: 10 mins

# July 8 2025
I updated the silkscreen a little bit now this is how it looks:  

![final pcb img](/images/8/pcb_final_3.png)  
![final cad 1](/images/8/3d_1_final_2.png)  
![final cad 2](/images/8/3d_2_final_2.png)  
![final sch img](/images/5/sch_final.png)  


Now i am gonna start writing the BOM and write more README and 

And i did very little stuff.
### Time Spent Today: 10 mins

# July 9 2025
Uhhhh i dont wanna procastinate but i wanna complete and submit asap, i still have to write the BOM for it fkjhadfjkshakjdsfhkj.    

oh wait, i just realised that if i order from JLC, the declared value will be 12 USD, which is too much which i can't pay, so i will have to switch to ordering the pcb and stencil from JLC and components form LCSC.

# July 11 2025:
worked a bit on the BOm today, made it completely and now gonna work on making all the other things for submission

### Time Spent Today: 45 mins 