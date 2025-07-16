# Raspberry Pi Magnetic PETG Case for Ender 3

A custom magnetic PETG case designed specifically for the Raspberry Pi Zero 2 W, featuring dual fan cooling, LED support, modular screen mount, and camera integration. This case is designed to mount securely to an Ender 3 3D printer for enhanced cooling, monitoring, and lighting capabilities.

## Why I Made This Project

I needed a reliable cooling solution for my Raspberry Pi Zero 2 W that was running Klipper firmware for my Ender 3 printer. The standard cases available didn't provide adequate cooling for the continuous operation required during long print jobs. I also wanted to add LED lighting, a screen mount for better monitoring, and camera integration for timelapses. The magnetic attachment system makes it easy to remove and maintain without tools, while the modular design allows for easy upgrades and modifications.

## Features

- **Magnetic Attachment**: Tool-less assembly using neodymium magnets for easy maintenance
- **Dual 30mm Fans**: Perfect cooling for the Raspberry Pi Zero 2 W during long print jobs
- **LED Integration**: WS2812B strip support for ambient lighting and SK6812 RGBW strips for printer illumination
- **Modular Screen Mount**: Compatible with Waveshare 4.3" HDMI LCD for monitoring
- **Camera Mount**: Adjustable Raspberry Pi Camera Module 3 mount for 4K timelapses
- **Sound Dampening**: Integrated foam ball holders for vibration reduction
- **Cable Management**: Dedicated cable routing holes and access points
- **Klipper Integration**: Smart magnet cover printing using Klipper firmware

## Project Pictures


### Screen Mount
![Screen Mount Assembly](https://github.com/user-attachments/assets/a43e7878-2c99-4ef9-893f-4b569aac001a)

### Camera Integration
![Camera Mount Assembly](https://github.com/user-attachments/assets/518eac79-77e2-416b-b378-e872ebfad1dc)

### LED Lighting System
<img width="847" height="1001" alt="image" src="https://github.com/user-attachments/assets/7326cf10-3d1c-447a-8738-962688b31810" />


## Wiring Diagram


![Wiring Diagram](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8f8846a695e038cd5c8294e7fe0daab3fec1c36e_image.png)


## Wiring Diagram

Since this project uses standard connections without a custom PCB, here's the comprehensive wiring setup:

```
Raspberry Pi Zero 2 W
├── GPIO 18 → WS2812B LED Strip Data (printer lighting)
├── GPIO 21 → SK6812 RGBW <img width="1018" height="674" alt="463837668-74d05153-4630-4f8c-87a0-d8d51d3b4930" src="https://github.com/user-attachments/assets/d8a1b71c-9329-4780-9d65-e9ff1aa41fdf" />
Strip Data 
├── 5V → WS2812B LED Strip VCC
├── External 5V → SK6812 RGBW Strip VCC
├── GND → WS2812B LED Strip GND
├── External GND → SK6812 LED Strip GND
├── GND → SK6812 RGBW Strip GND
├── Micro HDMI → Waveshare 4.3" LCD
├── Camera Port → Raspberry Pi Camera Module 3
├── 5v →  Fan VCC
├──  GND → Fan GND
└── Micro USB → Power Supply
```


## Bill of Materials (BOM)<img width="1018" height="674" alt="463837668-74d05153-4630-4f8c-87a0-d8d51d3b4930" src="https://github.com/user-attachments/assets/699dad79-dde0-4d9c-93ef-befc49b54471" />

| Item No. | Product Name | Amazon Link | Quantity | Cost (USD) | Notes | Running Total (USD) |
|----------|--------------|-------------|----------|------------|-------|---------------------|
| 1 | Transparent Polymaker PETG Filament | [Link](https://www.amazon.com/dp/B09DKMCNMW?tag=all3dptrx00131-20&th=1) | 1 | $22.99 | Clear PETG filament for 3D printing | $22.99 |
| 2 | WINSINN 30mm RGB Fan 5V (Pack of 4Pcs) | [Link](https://www.amazon.com/WINSINN-Hydraulic-Bearing-Brushless-30x10mm/dp/B087QDRKW9/) | 1 | $8.99 | RGB micro fans for electronics/3D printing | $31.98 |
| 3 | Waveshare 4.3inch Capacitive Touch Screen LCD | [Link](https://www.amazon.com/4-3inch-HDMI-LCD-Resolution-Capacitive/dp/B07MB9MYYS/) | 1 | $53.99 | Touch display compatible with Raspberry Pi | $85.97 |
| 4 | Neodymium Magnets 5mm x 3mm (60 Pack) | [Link](https://www.amazon.com/Magnets-Multi-use-Refrigerator-Neodymium-Whiteboard/dp/B0BJDZRHV7/) | 1 | $3.99 | Mini magnets for mounting and DIY | $89.96 |
| 5 | Raspberry Pi 5 | [Link](https://www.amazon.com/dp/B0DRRRZBMP?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_1) | 1 | $26.99 | Main single-board controller | $116.95 |
| 6 | SEZO WS2812B LED Strip Light 1M | [Link](https://www.amazon.com/SEZO-Individually-Addressable-Programmable-Non-Waterproof/dp/B097BX7LRT/) | 1 | $6.99 | Addressable RGB LED strip for effects | $123.94 |
| 7 | Ktehloy 400Pcs Threaded Inserts | [Link](https://www.amazon.com/mxuteuk-420PCS-Screws-Socket-Wrench/dp/B0CSWD34KJ/) | 1 | $13.49 | Brass heat-set inserts for plastic parts | $137.43 |
| 8 | mxuteuk M3 Screws Kit (420PCS) | [Link](https://www.amazon.com/TOP-VIGOR-Machine-Fastener-Motorcycle-Repairment/dp/B0D5CJXW8X/) | 1 | $9.99 | Assorted M3 screws for Pi and mounts | $147.42 |
| 9 | TOP-VIGOR M4-0.7 x 12mm Socket Screws (30PCS) | [Link](https://www.amazon.com/TOP-VIGOR-Machine-Fastener-Motorcycle-Repairment/dp/B0D5CJXW8X/) | 1 | $5.35 | Screws for camera mounting | $152.77 |
| 10 | Arducam Raspberry Pi Camera Module 3 | [Link](https://www.amazon.com/Arducam-Raspberry-Camera-Autofocus-15-22pin/dp/B0C9PYCV9S/) | 1 | $22.00 | 12MP autofocus camera for Pi | $174.77 |
| 11 | UeeKKoo DSI FPC Flexible Cable | [Link](https://www.amazon.com/UeeKKoo-Flexible-Raspberry-Display-Suitable/dp/B0D12TMQ6D/) | 1 | $4.99 | Ribbon cable for Raspberry Pi display | $179.76 |
| 12 | BTF-LIGHTING SK6812 RGBW LED Strip 1M | [Link](https://www.amazon.com/BTF-LIGHTING-Individually-Addressable-Flexible-Non-waterproof/dp/B079ZT9Q9X/) | 1 | $25.99 | RGBW LED strip with addressable control | $205.75 |
| 13 | Zugar Land Galaxy Foam Stress Balls (4 Pack) | [Link](https://www.amazon.com/Zugar-Land-Squeeze-Relaxable-Calming/dp/B0CZS91TNW/) | 1 | $6.99 | Stress relief or soft bumper component | $212.74 |

Total project development time: **23.5 hours**

