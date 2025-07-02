---
title: "Raspberry Pi Magnetic PETG Case — Ender 3 Cooling Mod"
author: "Tanishq Goyal"
description: "Custom magnetic PETG case with dual fan cooling, LED support, and modular screen mount for my Ender 3"
created_at: "2025-06-25"
---

# Raspberry Pi Magnetic PETG Case

**Total time spent: 21h**

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

**Total time spent: 3h**

---

# June 25th: Design Improvements

- Applied fillets for smoother corners  
  ![Fillets](https://github.com/user-attachments/assets/f08adb94-8b14-4f51-a1ed-7486d4a8843a)
  ![Fillet](https://github.com/user-attachments/assets/63ab9967-0384-4826-8ca9-1ecd3cd61dab)  

Added alignment tabs to ensure proper assembly and prevent misalignment:  
![Alignment Tab](https://github.com/user-attachments/assets/55e59318-e8b3-46a4-9afb-e8d176820762)  
![Tab Slot](https://github.com/user-attachments/assets/8d78f0bc-efd2-40da-b093-30ab285be5a5)

**Total time spent: 2h**

### 6/26/2025 

#### space for pi 
![Side Panel](https://github.com/user-attachments/assets/24354a62-7fb9-4df8-8bf4-b49d51dd03f6)

Designed the top cover to complete the enclosure:  
![Top Cover](https://github.com/user-attachments/assets/382b640b-e576-407e-bafa-faf6cd6786c1)

Added specific Pi mount holes for secure mounting:  
![RPi Holes](https://github.com/user-attachments/assets/a10bafca-de03-4d51-933a-a2e635011476)

**Total time spent: 2h**

---

## Cable Management

Removed material for easier cable access to make installation and maintenance simpler:  
![Cable Opening](https://github.com/user-attachments/assets/90cd0a44-a664-41f1-b0b8-834a8f0094bc)  
![Shaving Detail](https://github.com/user-attachments/assets/04eccf04-4a87-4f5b-8e0a-34f024239bc8)

Added proper cable holes for clean cable routing:  
![Cable Holes](https://github.com/user-attachments/assets/dbdd7ae3-2589-4436-8a20-fbb0d2a76995)

Here's how it looks assembled:  
![Assembled View](https://github.com/user-attachments/assets/1e37d00f-fcf2-43e2-a7d1-22d7578a734c)

**Total time spent: 3h**

---

## LED Integration

Planned to add rails for WS2812B LED strips to add some nice ambient lighting to the setup:  
![LED Rails](https://github.com/user-attachments/assets/73b76ade-cd06-446a-8979-976c9e1852ac)  
![More Rails](https://github.com/user-attachments/assets/97e43991-d02b-4c14-8b2b-1f5bcafa7527)

**Total time spent: 3h**

---

# June 27th: Screen Mount and LED Rail Redesign

Had some issues with the LED slide design initially. After brainstorming, I realized **neodymium magnets** could provide a sleek, clean, and removable attachment system for the LED strips.

![LED Rail Design](https://github.com/user-attachments/assets/078cb473-4579-43cc-a03d-5535191a0fc1)

**Total time spent: 1h**
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

**Total time spent: 5h**


# June 28th: I realised instead of gluing it in, I can print over it by simply adding a "stop" command in klipper!

Firs,t I added a variable of the amt of layers of PLA. For now, for 2 layers, im using 0.4 mm. With too much layers, im scared of loss of magnetic connection. Then, Ill just cover it as such:

![image](https://github.com/user-attachments/assets/6587d8e9-1090-4525-8269-6792d2dfc911)
![image](https://github.com/user-attachments/assets/fc2bb48c-292c-404d-9a8b-ca3882056373)


[insert pictures of what you're working on!]

**Total time spent: .5h**

6/29/2024

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
