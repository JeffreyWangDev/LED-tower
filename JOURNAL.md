---
title: LED-Tower
author: Jeffrey
description: Simple, good looking led light 
created_at: 7-4-2025
---




## Day One
**5 hours**

I found an example of something that I want to make it look like ![image](https://github.com/user-attachments/assets/07b93cf5-7b04-4af0-b82a-26b26e9146a9)

Problems with this that I have,
1. Too dim
2. Looks to be non addresable LEDS
3. Made with a 2 by 4?????
4. External LED driver/PSU
5. No USB-C charging ports

Pros:
1. The acrylic that they have is so clear
2. I love the beveled edges, good idea


After looking online for a bit I started to design the tower part of the build, I made a simple model
![image](https://github.com/user-attachments/assets/2daa114d-ade6-4bef-bf8d-6a9d01e891fd)


After this, I was stuck with problem one: how should I attach the acrylic panels to the tower? I thought about different ways, including epoxy, regular glue, pressure fit, screws into the acrylic, a rod that comes from above and goes though all of the pieces, and a nut inside the acrylic and a bolt behind it.    
I really don't want to use epoxy because that makes it impossible to disassemble and move, same with the glue, so those two are out. Pressure fit will work, but I don't know how secure that will be, and that requires really tight tolerances. Screws into the acrylic will work but I want to use a laser/2.5d cnc to cut the acrylic so thats not an options. A rod from above works, but I also don't know how secure that will be. 
Because of all of this, I decided to go with the nut-and-bolt way. The amount of time I spent thinking about attaching two things together is too crazy; I never want to do that again.


After that dilemma, I decided to call it quits for today.


## Day Two
**8 hours**

This day was mostly the onshaping work. I designed the acrylic pieces with the above-mentioned mounting way (See below for images). I also designed the main tower part of the build that holds everything together. In doing so, I learned about a cool feature called linear patterns and loved using it. The main tower needs to hold the acrylic, a PCB for the LEDs, and a backing plate. 
To hold the acrylic pieces in, I have bolt holes in the image below in orange. These are not going to be tapped and only used for holding the acrylic in. These use m3 by 16 bolts, which I have some at home and some at FTC that I can steal (tehe). The square holes are for the LEDs to shine into the acrylic and are spaced 2.5cm apart. The holes in the center are used for holding the PCB. 
I also have a photo below of the image of the back of the tower with raised studs for the PCB to sit on.


![image](https://github.com/user-attachments/assets/5bbe4555-9f2d-4f32-91ee-93988207c821)
![image](https://github.com/user-attachments/assets/36a8f9cb-f653-4849-9131-ffb76b03a43c)
![image](https://github.com/user-attachments/assets/2818969e-dfd2-4274-a1c5-579d9c7e04d7)
![image](https://github.com/user-attachments/assets/84118860-4465-4402-a81a-afb978ce1a65)
![image](https://github.com/user-attachments/assets/bc493ef9-d0f1-4106-8acc-18b854b9a5f5)
![image](https://github.com/user-attachments/assets/6f875d59-d402-4f5b-93ae-3c09c5946162)


## Day Three
**6 hours** 

Today I wanted to finish the LED PCB and start thinking about the base PCB. 
Have 50 LEDs with capacitors on the LED board, and I also have solder points for pwr and ground.
While the schematic was very easy, laying out the componets was way harder than I thought it would be. There is NO place tool in EasyEDA, so every component needs to be added by hand. This was taking literally forever, and I even started developing a script that places them for me, but gave up trying to read the documentation, which was ALL in Chinese. I'm literally Chinese but still can't read it, kinda disappointing (on me, not the devs). 

Read alot about USB-PD and different chips that I would need, will figure it out when I'm less dead. Done with day 3.

![image](https://github.com/user-attachments/assets/3abfdad2-be8b-4125-80ea-9c9baf1d36c3)
![image](https://github.com/user-attachments/assets/2854e4d1-7dbd-424c-8ce3-1eef9f81a07d)

## Day Four
**8 hours**

Spent around 4 hours reading up on the USB 3.0 standard, reviewing datasheets for PD source ICs, and searching for schematics to reference. In the end, it was all for nothing. I found a chip from an old design that supports USB PD that JLCPCB can actually make. This was a big problem because many of the newer USB-PD control ICs are not on LCSC, meaning that I could not use JLC to assemble the PCBs. This IC combines both the PD delivery and the buck converter, which makes it very easy to wire up. I made a PCB for that, and I also read the CNC guidelines and restrictions, and I changed the design for the front piece to allow for it to be CNCed. CNC aluminum is so much better looking and stronger than 3d printed parts. 
![image](https://github.com/user-attachments/assets/2292479b-f594-45d3-aca1-f433ae9dd5e6)
![image](https://github.com/user-attachments/assets/a409ea61-b763-4040-92fb-fadf48635225)

## Day Five
**3 hours**


Quickly made the control PCB for the LEDS. This PCB has the ESP32 and the 5V buck converter to convert 15V to 5V.  
This can also work as a dev board if needed.
![image](https://github.com/user-attachments/assets/e84e32f3-4c62-4bf0-8277-8c2ad3e505e8)
![image](https://github.com/user-attachments/assets/265e89b8-681c-4fce-917a-61d5948ce794)

## Day Six
**4 hours**

Remade the base PCB to have both usb-pd and control into one to save on costs. I also worked on the top tower, made a back, and updated holes/more. 


<img width="383" height="1067" alt="image" src="https://github.com/user-attachments/assets/fd0135da-9cf7-4355-b43e-0925da61e0f6" />
<img width="601" height="1049" alt="image" src="https://github.com/user-attachments/assets/1fb2c76f-4852-43e4-b06d-7ba5009e1581" />



## Day Seven
**6 Hours**

Made the base of the tower. This has all the control and power for the LEDs + USB-C ports. 


<img width="1588" height="838" alt="image" src="https://github.com/user-attachments/assets/6377c380-4c94-497e-889a-aac9d696da3e" />
<img width="1282" height="552" alt="image" src="https://github.com/user-attachments/assets/725896af-79f0-40a0-b1e1-d3c96f997664" />


<img width="597" height="357" alt="image" src="https://github.com/user-attachments/assets/6b9458b3-beed-4add-a0cb-492d7335e645" />
<img width="1396" height="854" alt="image" src="https://github.com/user-attachments/assets/90cfe158-01e9-4e87-8fac-202b8537fac7" />
<img width="1372" height="1052" alt="image" src="https://github.com/user-attachments/assets/bae18e9b-a601-4988-a68e-7bd69d50c8c0" />


## Day Eight + Nine
**12 Hours**

Today, I took a small model of the tower that I built out of wood and some random pieces of leftover polycarbonate and used it to test out the mounting for the acrylic. My fears about the glue were correct, and the wood is not strong enough to hold up the acrylic. I don't have design files cause I kinda just bought wood and acrylic with a hacksaw, but I attached photos down below. A problem that I ran into was not accounting for some small differences in the glue, but the CNCed part with nuts and bolts should not have the same problem. I never got it to power up, probably due to my burning the PSU and the LED controller that I had. I also adjusted many tolerances in Onshape, took forever cause I set up my dimension wrong the first time.

<img width="403" height="611" alt="image" src="https://github.com/user-attachments/assets/53ab6422-9b76-48ae-af2d-cfa00ed96493" />
