# Raspberry Pi Magnetic PETG CasE
A custom magnetic PETG case designed specifically for the Raspberry Pi Zero 2 W, featuring dual fan cooling, LED support, and a modular screen mount. This case is designed to mount securely to an Ender 3 3D printer for enhanced cooling and monitoring capabilities.

## Why I Made This Project

I needed a reliable cooling solution for my Raspberry Pi Zero 2 W that was running Klipper firmware for my Ender 3 printer. The standard cases available didn't provide adequate cooling for the continuous operation required during long print jobs. I also wanted to add LED lighting and a screen mount for better monitoring and aesthetics. The magnetic attachment system makes it easy to remove and maintain without tools.

## Features

- **Magnetic Attachment**: Tool-less assembly using neodymium magnets
- **Dual 30mm Fans**: Perfect cooling for the Raspberry Pi Zero 2 W
- **LED Integration**: WS2812B strip support for ambient lighting
- **Modular Screen Mount**: Compatible with Waveshare 4.3" HDMI LCD
- **Cable Management**: Clean routing with dedicated cable holes
- **PETG Construction**: Durable and heat-resistant material

## Project Pictures

### Full 3D Model Screenshot
![Full 3D Model](https://github.com/user-attachments/assets/7a48b7cb-0c8e-43d6-abef-eef99822f65b)

### Assembled View
![Assembled View](https://github.com/user-attachments/assets/1e37d00f-fcf2-43e2-a7d1-22d7578a734c)

### Case Components
![Case Components](https://github.com/user-attachments/assets/78e39d88-5e31-4a4e-aadd-7964a1cf9395)

### LED Rail Design
![LED Rail Design](https://github.com/user-attachments/assets/078cb473-4579-43cc-a03d-5535191a0fc1)

### Screen Mount
![Screen Mount](https://github.com/user-attachments/assets/b3930237-78b4-4646-a187-238d99199a52)

## Wiring Diagram

Since this project uses standard connections without a custom PCB, here's the wiring setup:

```
Raspberry Pi Zero 2 W
├── GPIO 18 → WS2812B LED Strip Data
├── 5V → WS2812B LED Strip VCC
├── GND → WS2812B LED Strip GND
├── Micro HDMI → Waveshare 4.3" LCD
└── Micro USB → Power Supply

30mm Fans (2x)
├── 5V → Fan VCC
└── GND → Fan GND
```

## Installation

1. **Print the Case Parts**: Use PETG filament for best results
2. **Insert Magnets**: Press neodymium magnets into the designated holes
3. **Mount Raspberry Pi**: Secure the Pi using M3 screws and heat set inserts
4. **Install Fans**: Connect and mount the 30mm cooling fans
5. **Add LED Strip**: Mount WS2812B strip to the magnetic rails
6. **Attach Screen**: Mount the Waveshare LCD to the screen mount
7. **Connect Cables**: Route all cables through the designated holes

## CAD Source Files

The CAD source files are located in the `cad/` directory:
- `case_main.step` - Main case body
- `case_top.step` - Top cover
- `screen_mount.step` - Screen mounting bracket
- `led_rails.step` - LED strip mounting rails
- `fan_grill.step` - Fan protection grill

## Bill of Materials (BOM)

| Item | Description | Quantity | Part Number | Supplier | Notes |
|------|-------------|----------|-------------|----------|-------|
| 1 | Raspberry Pi Zero 2 W | 1 | RPI-ZERO2-W | Official Raspberry Pi Store | Main computer board |
| 2 | 30mm x 30mm Cooling Fan | 2 | 30x30x10mm | Amazon/Adafruit | Dual fans for cooling |
| 3 | Neodymium Magnets (6mm x 2mm) | 8 | N35-6x2mm | Amazon | For magnetic attachment |
| 4 | WS2812B LED Strip | 1 | WS2812B-60LED/m | Adafruit/Amazon | RGB lighting |
| 5 | Waveshare 4.3" HDMI LCD-B | 1 | 4.3inch-HDMI-LCD-B | Waveshare | Display screen |
| 6 | PETG Filament (1.75mm) | 1 | 1kg spool | Any 3D printer supplier | For 3D printing case parts |
| 7 | M3 Screws (10mm) | 4 | M3x10 | McMaster-Carr | For mounting components |
| 8 | M3 Nuts | 4 | M3 | McMaster-Carr | For securing screws |
| 9 | Micro HDMI Cable | 1 | Micro HDMI to HDMI | Amazon | For screen connection |
| 10 | Micro USB Cable | 1 | Micro USB to USB | Amazon | For power supply |
| 11 | GPIO Header Pins | 1 | 40-pin header | Adafruit | For LED strip connection |
| 12 | Heat Set Inserts (M3) | 4 | M3 heat set | McMaster-Carr | For threaded inserts in 3D printed parts |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by the need for better cooling solutions for 3D printer control systems
- Thanks to the Klipper community for firmware support
- Special thanks to Waveshare for the LCD display specifications 
