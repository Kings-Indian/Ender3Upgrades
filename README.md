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

### Main Case and Screen Assembly
![Main Case Layout](https://github.com/user-attachments/assets/5af6afa8-bf43-4eae-879b-342f3800ba49)
)

### Camera Integration
![image](https://github.com/user-attachments/assets/51e10a9a-5f24-45f4-b114-72786f383d59)

![image](https://github.com/user-attachments/assets/6af93df9-b87d-4129-8cf3-f349af5c587f)



## Wiring Diagram

Since this project uses standard connections without a custom PCB, here's the comprehensive wiring setup:

```
Raspberry Pi Zero 2 W
├── GPIO 18 → WS2812B LED Strip Data
├── GPIO 21 → SK6812 RGBW Strip Data (printer lighting)
├── 5V → WS2812B LED Strip VCC
├── 5V → SK6812 RGBW Strip VCC
├── GND → WS2812B LED Strip GND
├── GND → SK6812 RGBW Strip GND
├── Micro HDMI → Waveshare 4.3" LCD
├── Camera Port → Raspberry Pi Camera Module 3
└── Micro USB → Power Supply

30mm Fans (2x)
├── 5V → Fan VCC
└── GND → Fan GND

Camera Module 3
└── Camera Port → Raspberry Pi Zero 2 W
```

## Installation

1. **Print the Case Parts**: Use PETG filament for best results and durability
2. **Insert Magnets**: Press neodymium magnets into the designated holes
3. **Mount Raspberry Pi**: Secure the Pi using M3 screws and heat set inserts
4. **Install Fans**: Connect and mount the 30mm cooling fans
5. **Add LED Strips**: Mount WS2812B strip to the magnetic rails and SK6812 strip to the printer
6. **Attach Screen**: Mount the Waveshare LCD to the screen mount
7. **Install Camera**: Mount the Raspberry Pi Camera Module 3 to the adjustable mount
8. **Add Sound Dampening**: Install foam balls in the designated holders
9. **Connect Cables**: Route all cables through the designated holes
10. **Configure Klipper**: Set up the magnet cover printing parameters

## CAD Source Files

The CAD source files are available in the `cad/` directory:
- `case_main.step` - Main case body
- `case_top.step` - Top cover with screen mount
- `fan_grill.step` - Fan grill design
- Additional components available upon request

## Bill of Materials (BOM)

| Item | Description | Quantity | Part Number | Supplier | Notes |
|------|-------------|----------|-------------|----------|-------|
| 1 | Raspberry Pi Zero 2 W | 1 | RPI-ZERO2-W | Official Raspberry Pi Store | Main computer board |
| 2 | 30mm x 30mm Cooling Fan | 2 | 30x30x10mm | Amazon/Adafruit | Dual fans for cooling |
| 3 | Neodymium Magnets (6mm x 2mm) | 8 | N35-6x2mm | Amazon | For magnetic attachment |
| 4 | WS2812B LED Strip | 1 | WS2812B-60LED/m | Adafruit/Amazon | RGB lighting for case |
| 5 | SK6812 RGBW LED Strip | 1 | SK6812-144/m | BTF-LIGHTING | Printer illumination |
| 6 | Waveshare 4.3" HDMI LCD-B | 1 | 4.3inch-HDMI-LCD-B | Waveshare | Display screen |
| 7 | Raspberry Pi Camera Module 3 | 1 | Camera Module 3 | Official Raspberry Pi Store | 4K timelapse camera |
| 8 | PETG Filament (1.75mm) | 1 | 1kg spool | Any 3D printer supplier | For 3D printing case parts |
| 9 | M3 Screws (10mm) | 6 | M3x10 | McMaster-Carr | For mounting components |
| 10 | M3 Screws (40mm) | 1 | M3x40 | McMaster-Carr | For camera mount |
| 11 | M3 Nuts | 6 | M3 | McMaster-Carr | For securing screws |
| 12 | Micro HDMI Cable | 1 | Micro HDMI to HDMI | Amazon | For screen connection |
| 13 | Micro USB Cable | 1 | Micro USB to USB | Amazon | For power supply |
| 14 | GPIO Header Pins | 1 | 40-pin header | Adafruit | For LED strip connection |
| 15 | Heat Set Inserts (M3) | 4 | M3 heat set | McMaster-Carr | For threaded inserts |
| 16 | Foam Balls (2 inch) | 4 | 2" foam balls | Amazon | Sound dampening |
| 17 | Camera Cable | 1 | Camera Module 3 cable | Official Raspberry Pi Store | Camera connection |

## Technical Specifications

- **Case Material**: PETG (Polyethylene Terephthalate Glycol)
- **Print Settings**: 0.4mm nozzle, 0.2mm layer height, 100% infill for structural parts
- **Magnetic Force**: N35 neodymium magnets provide secure attachment
- **Camera Mount**: Adjustable ±20° rotation for optimal positioning
- **LED Integration**: WS2812B for case lighting, SK6812 RGBW for printer illumination
- **Sound Dampening**: 2-inch foam balls reduce vibration and noise
- **Compatibility**: Ender 3 series printers with 2020 extrusion profiles

## Development Time

Total project development time: **23.5 hours**
- Design and modeling: 15 hours
- Testing and refinement: 5 hours
- Documentation and optimization: 3.5 hours
