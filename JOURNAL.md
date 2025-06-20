---
title: "A BLDC and driver"
author: "Sophia"
description: "A brushless dc motor and a driver for it"
created: "2025-06-13"
---
# June 13th: Began my PCB and fixed my CAD model

**Total time spent: ~5h**

This is a continuation of my project from physics class. I originally cadded the motor with bad tolerances and poor alignment between the magnets and coils and had nothing to drive it.
So it was really a pile of 3D printed crap. 

Now I plan on completely fixing all the models and make a custom PCB to drive it (with PWM) 

Today I recadded the motor and worked on a basic schematic
![image](https://github.com/user-attachments/assets/b18d0699-c844-4d04-8c96-410b34224612)

![image](https://github.com/user-attachments/assets/cd8bc1e1-d3f9-4139-9f9d-40f303253915)
![image](https://github.com/user-attachments/assets/1df7d0f2-cb2c-4179-9653-132d3f8a3a28)

^ a section view because I just learned how to do that recently and its super epic
This is just the start of the schematic, right now the driver design is super basic. It's a discrete driver meaning its not using any IC's. Later, once school is over i'll add some more unique and practical features to it.

Side note: My kiCAD wakatime kept on not working, and i don't think fusion 360 has wakatime 😔

# June 14th: Planning and added small features

**Total time spent: 20mins**


![image](https://github.com/user-attachments/assets/724de8ed-ba91-471f-956a-3230b34abac0)


I added a few buttons and LEDs which in the future will turn the board on/off, reverse direction and LEDs to display statuses. I think I am missing a few more small ones. 
I really didn't have much time today but I did brainstorm some features I want this to have:
- an case for the pcb
- smooth start-up
- more sockets for testing purposes
- make it safe / protect it
- make it compatible with most commercial bldcs 

# June 16th: New plan

**Total time spent: 3h**
Most of the time spent this session was researching, which is where I learned about the VESC which will be super helpful for the firmware

I decided on using an OLED display and a esp32 to control it, this will show the user the RPM, V, current draw...

I researched what MCU to use and settled on the STM32F405RGTx

![image](https://github.com/user-attachments/assets/9dc22619-1810-46ed-aa8b-4189a6775cc2)

First time using hierarchal sheets + labels and modified my V1 schematic for the new components and separated them
