---
title: "Raspberry Pi Magnetic PETG Case — Ender 3 Cooling Mod"
author: "Tanishq Goyal"
description: "Custom magnetic PETG case with dual fan cooling, LED support, and modular screen mount for my Ender 3"
created_at: "2025-06-25"
---

# Raspberry Pi Magnetic PETG Case

**Total time spent: 24.5h**

## Goal
Design and print a custom **PETG case for my Ender 3** focused on cooling and modularity.  
Key features:
- Magnetic attachment for easy assembly
- Dual 30mm fans (perfect match for the 30mm × 65mm Raspberry Pi Zero 2 W)
- LED support with WS2812B strips
- Modular screen mount

---

# June 25th: Initial Layout and Planning

Started the design process by planning the overall layout for the Raspberry Pi case. The goal was to create a magnetic PETG case that would fit perfectly on my Ender 3 with dual fan cooling.

This setup allows this layout:

![Layout](https://github.com/user-attachments/assets/7193a171-dd17-445b-868b-73dc5ac8ab1e)

Designed the fan case conforming with this layout:  
![Fan Case](https://github.com/user-attachments/assets/78e39d88-5e31-4a4e-aadd-7964a1cf9395) 

Added holes to embed **neodymium magnets** for tool-less assembly:  
![Magneto](https://github.com/user-attachments/assets/c47df648-fc2f-4a52-8aad-9ebf089d2874)
![Neodymium Magnets](https://github.com/user-attachments/assets/60aa222c-18e8-44f1-af43-2551c76b5584)

**Total time spent: 2h**

---

# June 25th: Design Improvements

- Applied fillets for smoother corners  
  ![Fillets](https://github.com/user-attachments/assets/f08adb94-8b14-4f51-a1ed-7486d4a8843a)
  ![Fillet](https://github.com/user-attachments/assets/63ab9967-0384-4826-8ca9-1ecd3cd61dab)  

Added alignment tabs to ensure proper assembly and prevent misalignment:  
![Alignment Tab](https://github.com/user-attachments/assets/55e59318-e8b3-46a4-9afb-e8d176820762)  
![Tab Slot](https://github.com/user-attachments/assets/8d78f0bc-efd2-40da-b093-30ab285be5a5)

**Total time spent: 1h**

---

# June 26th: Raspberry Pi Space and Top Cover

#### space for pi 
![Side Panel](https://github.com/user-attachments/assets/24354a62-7fb9-4df8-8bf4-b49d51dd03f6)

Designed the top cover to complete the enclosure:  
![Top Cover](https://github.com/user-attachments/assets/382b640b-e576-407e-bafa-faf6cd6786c1)

Added specific Pi mount holes for secure mounting:  
![RPi Holes](https://github.com/user-attachments/assets/a10bafca-de03-4d51-933a-a2e635011476)

**Total time spent: 1h**

---

# June 26th: Cable Management

Removed material for easier cable access to make installation and maintenance simpler:  
![Cable Opening](https://github.com/user-attachments/assets/90cd0a44-a664-41f1-b0b8-834a8f0094bc)  
![Shaving Detail](https://github.com/user-attachments/assets/04eccf04-4a87-4f5b-8e0a-34f024239bc8)

Added proper cable holes for clean cable routing:  
![Cable Holes](https://github.com/user-attachments/assets/dbdd7ae3-2589-4436-8a20-fbb0d2a76995)

Here's how it looks assembled:  
![Assembled View](https://github.com/user-attachments/assets/1e37d00f-fcf2-43e2-a7d1-22d7578a734c)

**Total time spent: 3h**

---

# June 26th: LED Integration

Planned to add rails for WS2812B LED strips to add some nice ambient lighting to the setup:  
![LED Rails](https://github.com/user-attachments/assets/73b76ade-cd06-446a-8979-976c9e1852ac)  
![More Rails](https://github.com/user-attachments/assets/97e43991-d02b-4c14-8b2b-1f5bcafa7527)

**Total time spent: 3h**

---

# June 27th: Screen Mount and LED Rail Redesign

Had some issues with the LED slide design initially. After brainstorming, I realized **neodymium magnets** could provide a sleek, clean, and removable attachment system for the LED strips.

![LED Rail Design](https://github.com/user-attachments/assets/078cb473-4579-43cc-a03d-5535191a0fc1)

**Total time spent: 1h**

---

# June 27th: Screen Mount Design

For the screen, I couldn't find the exact model online. I based my design on this similar model. While I am using 
[Waveshare 4.3" HDMI LCD-B](https://www.waveshare.com/4.3inch-HDMI-LCD-B.htm), the model is of https://www.waveshare.com/4.3inch-dsi-lcd.htm
![image](https://github.com/user-attachments/assets/b7ad5964-fbdf-43c8-bb91-b195f933497e)

Added a **10mm margin** on all sides, with a cutout on the right and top for cable clearance:  
![image](https://github.com/user-attachments/assets/b3930237-78b4-4646-a187-238d99199a52)  
![image](https://github.com/user-attachments/assets/61ea1794-9dbd-473c-90fe-ebcfc4da5365)

To enclose the top, I refined the model to match the screen's plane:  
![image](https://github.com/user-attachments/assets/f035eaf7-d4e4-4ca0-8762-4102c2b7db6a)

After applying **fillets to all edges**, final design complete:  
![image](https://github.com/user-attachments/assets/7a48b7cb-0c8e-43d6-abef-eef99822f65b)  
![image](https://github.com/user-attachments/assets/a43e7878-2c99-4ef9-893f-4b569aac001a)

**Total time spent: 2h**

---

# June 28th: Klipper Integration for Magnet Covers

I realised instead of gluing it in, I can print over it by simply adding a "stop" command in klipper!

Firs,t I added a variable of the amt of layers of PLA. For now, for 2 layers, im using 0.4 mm. With too much layers, im scared of loss of magnetic connection. Then, Ill just cover it as such:

![image](https://github.com/user-attachments/assets/6587d8e9-1090-4525-8269-6792d2dfc911)
![image](https://github.com/user-attachments/assets/fc2bb48c-292c-404d-9a8b-ca3882056373)

[insert pictures of what you're working on!]

**Total time spent: 0.5h**

---

# June 29th: Design Refinements

I realised how bad this cover is. I believe it deserves more love
![image](https://github.com/user-attachments/assets/d6439985-69f3-470a-b89c-7e9e84a51a1c) (this one is fine )

Since there just for allignment, ill make them much smaller and farther form the magnets.
I redid that part with a simular idea:
![image](https://github.com/user-attachments/assets/2b77f6b4-1c7e-4880-9d6c-62e1e3304eb3)

I also realized how hard it is to read, so I reorganized the features
![image](https://github.com/user-attachments/assets/f49b9b99-1076-4ce4-8964-c0adc00100e1)

![image](https://github.com/user-attachments/assets/88f8aea3-d8e9-42e5-b962-135b6715a6ea)

I then fixed up the assembly once more:

![image](https://github.com/user-attachments/assets/6e07dfd6-8b01-4877-a369-e2f6e5e0fa34)

![image](https://github.com/user-attachments/assets/89b34f58-6893-455c-9d8f-89ca73dbde79)

**Total time spent: 1.5h**

---

# June 29th: Camera Mount Planning

I also decided to add camera mounts and leds to the printer for lighting.
After a lot of thought, I will start modeling the Rasberry Pi 3 camera mount. Although the right side is easier to model with, soley due to my current setup I am modeling everything on the left. 
First, I incrased the space it has for flexability and for the SD Card and camera. 

After looking at joints, it seems a typical butt hinge and other common hinges arent good for my purpose (based off https://www.youtube.com/watch?v=fbY7xHGaeNM.) I will try to make a design similar to a normal door hinge to increase traction, allowing the pi to be held in place:

![image](https://github.com/user-attachments/assets/2f6b576b-b802-4e60-9075-0554eb48dc3d)

First, I decided to keep it only rotatable on the z axis. There was no real reason I saw I would want motion on the Y axis, since I want the nozzle always centered. I also wanted to keep the camera from hitting the toolhead, the FOV from seeing the Z Pole , and planned to mount it to the tensioner. This transalates to my sketch:

![image](https://github.com/user-attachments/assets/591efda1-2ded-412c-b51e-458ace88fff1)|
I am accounting for the space betweeb the lense and back of the pi as tolerance for the pi not hitting the z Gantry. 

I chose the Raspberry Pi Camera Module 3 over the other Pi models because it delivers sharper 4K timelapses, handles low-light printing conditions better with its f/1.8 aperture, and offers autofocus flexibility. Due to the 120 Percent fov, I ex pect to angle it at about 60 sdegrees. For adjustments I still want the ability to rotat ed on the Z Axis. 

![FOV at 60 degrees](https://github.com/user-attachments/assets/3c99858a-5a5b-43f2-a401-7f626624580e)

Regardless, I will design this at 90 degrees for now since rotation is always possible. 

**Total time spent: 2h**

---

# July 6th: Camera Mount Design

I decided to model it at the 20 degrees (I saw the FOV wrong) with 20 degrees of mobility in both directions. Long term, I will likely use a non adjustAbble mount 

Updated sketches:
![image](https://github.com/user-attachments/assets/4bc09044-54cc-467c-9d37-e61a9420f7b3)
![image](https://github.com/user-attachments/assets/122d9e17-44d8-41d4-845a-621c19db34a9)

![image](https://github.com/user-attachments/assets/b43f7638-5f44-480a-8904-7bd8307048be)
![image](https://github.com/user-attachments/assets/0d64517b-e438-48f3-81fe-becbb1f6438c)
This mount lets me hasve a strong connection while letting me rotated the needed amount|

This is the fional roptating camera mount
![image](https://github.com/user-attachments/assets/404f0453-2af2-407c-8ca0-16a1fee1cf67)

Hole for RPI Camera:

![image](https://github.com/user-attachments/assets/d83feb99-841e-495e-b23c-82cb81ca683e)

I will fasten it with a 40 mm m3 screw

![image](https://github.com/user-attachments/assets/1564c699-4e36-489c-aacd-cf5f6c2bc5e8)

**Total time spent: 2h**

---

# July 7th: Camera Mount Finalization

This is the finalized rotating camera mount
![image](https://github.com/user-attachments/assets/518eac79-77e2-416b-b378-e872ebfad1dc)

![image](https://github.com/user-attachments/assets/01cd4079-1078-4be7-a004-1467fdb96dfb)

I decided to change tghe adjustabilty so the bottom angle is 20 degrees isnteadof 40:

![image](https://github.com/user-attachments/assets/308a7edf-a3ff-4d6b-9980-6bc48546c4bf)

![image](https://github.com/user-attachments/assets/cdfdac68-9f58-4746-a88d-dfe72d2ad9f8)

![image](https://github.com/user-attachments/assets/81517231-412d-49c0-a2d2-6594ed60dee3)
There isnt a danger opf the mount hitting the borttom extrusion, as there is only 16 mm of difference in the z axis:

![image](https://github.com/user-attachments/assets/03ff13d4-ff27-4137-99e8-04d705fccd87)
![image](https://github.com/user-attachments/assets/3793117a-9fd4-4d8c-a075-8072e004023b)
with the klipepr case:
![image](https://github.com/user-attachments/assets/0a299eec-3c20-47ad-8371-43db64de69b2)

now I just need to add LEDS for the Ender 3 top 2020 profile bar:

<img width="454" alt="image" src="https://github.com/user-attachments/assets/cefeb302-0130-4c77-be70-3b9e9bd9bca8" />

Since it should be bright, lighting up the build plate, I will use SK6812 leds due to its dedicated white channel for better white light (more clear video)

although I can thread it through the 2020 profile (its 10 mm, thus fitting within the 10.420mm indent of the profiles) I thought a dedicated LED sleeve would make more sense, as it would be more directly over the toolhead. This is roughly 50 mm of distance from the extrusion.

The profile is very confusing. After a lot of researched I stumbled upon cad which I would use for the lights to see how much the hole which lets the lwds be seeb has to be. However, it doesnt seem to be for tthese given the visual scale (led dimensions are Product Dimensions:1000x2.13x12.0mm in https://www.amazon.com/BTF-LIGHTING-Individually-Addressable-Flexible-Non-waterproof/dp/B01MYV70QZ/ref=sr_1_4?crid=37E7K9IZQ6H7Z&dib=eyJ2IjoiMSJ9.hL7R35l27nGH6psUWgDquHFFf2hV3_F21tSlMqPORj598Mfaxul4TXNkmTW24etIWAL3LQ0KukuIRpxwqBH6DDz-2liRkneLLfWTymthFOkEA_ioIsvTKs3bkDdqh_MxwJhQhAj2JYA8ZSp6Sf9UMw.qgj4Hrbxp0vZwfdZGWjqvDBU1gNlE2L1JOaBd-XSdIY&dib_tag=se&keywords=sk6812%2Brgbw%2B144%2Fm%2Bip65&qid=1751925181&refinements=p_85%3A2470955011&rnid=2470954011&rps=1&sprefix=SK6812%2B144%2B%2Caps%2C162&sr=8-4&th=1):

![image](https://github.com/user-attachments/assets/3c78fc2a-9fd9-4baa-9ed5-3ca142c86d8e)
![image](https://github.com/user-attachments/assets/c6d0ec7b-7e9b-4d93-aee1-7688dc033a61)
![image](https://github.com/user-attachments/assets/d519e0eb-67c0-4434-bfa5-d6af82352fcc)

Instead, ill assume the led is 8mm wide. While its nto best cad practice, I dont think i havea  better option and it shouldnt matter too much:

![image](https://github.com/user-attachments/assets/74b2d59b-9dec-4fe2-8233-99d934a55483) (while height dimensions might be wrong, for my purposes, it shouldnt matter. I plan to give it a 3 mm hole regardless. )

![image](https://github.com/user-attachments/assets/254fa1c6-ca1e-4aef-aa12-4c87112c7409)

I spent a while trying to figure it out but for some reaon the sketch would be solid so i just used the use feature to make ti solid in a different sketch:

![image](https://github.com/user-attachments/assets/04ed853a-66fd-4f03-8fa6-412bcfca1c18)

![image](https://github.com/user-attachments/assets/afb74036-e45e-46fc-bf76-3069dacd74a5)

for printing, ill split it into 2 even blocks. Ill also enclose one end on the shelf:![image](https://github.com/user-attachments/assets/75541b46-d703-4c5d-9f17-d124435f975b)

![image](https://github.com/user-attachments/assets/051449a2-3d91-4ace-96af-2e70fc26d737)

After applying fillets, it should be done:
![image](https://github.com/user-attachments/assets/bc417eec-dc10-4ed7-b65b-c22badb7a069)

<img width="397" alt="image" src="https://github.com/user-attachments/assets/70696913-9932-4444-a801-dac6a6eb2029" />

![image](https://github.com/user-attachments/assets/4d950745-fe28-412c-8d15-13398029e5e2)

**Total time spent: 3h**

---

# July 7th: Wiring and LED Integration

beyond this, all I have left is wiring. First, I will create a hole in the RPI case for the SK6812 LEDS:

![image](https://github.com/user-attachments/assets/894ebd59-03f5-4807-a5d5-a17b538ea2ed)
![image](https://github.com/user-attachments/assets/3048d6f1-7ba9-4eb1-a7ba-34f0ae8cfae9)
![image](https://github.com/user-attachments/assets/1b5b1a5b-f755-4968-8db6-a2257a0c1940)

**Total time spent: 1h**

---

# July 8th: Sound Dampening with Foam Balls

I decided to add measures against the high sounds the printer creates, as it makes it harder for me to sleep. First, I decided to add 2 inch foam balls, due to therir springiness and ability to absorb viberations. 

Here is the foam ball holder![image](https://github.com/user-attachments/assets/72a8365b-ce27-410d-bf5d-f75b7c9de5d7)
![image](https://github.com/user-attachments/assets/874b3abc-b610-4914-b341-641d7fd171d8)
![image](https://github.com/user-attachments/assets/74d05153-4630-4f8c-87a0-d8d51d3b4930)

**Total time spent: 1h**
8/1/25

turns out I caznt drill, 3d printing this thing 

<img width="1166" height="783" alt="image" src="https://github.com/user-attachments/assets/8a466718-4e53-484f-b256-ec8dbc8abaf3" />
<img width="684" height="614" alt="image" src="https://github.com/user-attachments/assets/37d596cf-59b5-4c84-aea3-8a056f0ae5e3" />

time spent: 1h


