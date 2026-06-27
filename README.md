# GeekMagic SmallTV-Ultra - Desktop Controller

A Windows desktop app to control your **GeekMagic SmallTV-Ultra** smart display from your PC - no browser required.

![Platform](https://img.shields.io/badge/platform-Windows-blue) ![Device](https://img.shields.io/badge/device-GeekMagic--SmallTV--Ultra-green)

---

## Features

### Display & Clock
- Switch between display themes (weather, clock, photo album, etc.)
- Adjust screen brightness and night mode brightness
- Set timezone, time format (12h/24h), date format, NTP server
- Customize clock font, colon blink, and RGB color

### Photo Album
- Upload photos directly from your PC - auto-cropped and resized to 240×240
- Upload animated GIFs for full-screen playback
- Set any image or GIF as the active display
- Delete individual files or clear the entire album
- Configure slideshow speed and transition settings

### Weather
- Set your city by name or city ID
- Configure temperature, wind speed, and pressure units
- Set weather update interval
- Upload custom 80×80 animated weather GIFs
- Enter your own OpenWeatherMap API key for a higher update rate

### Image & GIF Editor
- Crop and zoom before uploading - drag to reposition, scroll wheel to zoom
- Adjust brightness, contrast, saturation, and sharpness
- **GIF compression controls** - set max colors and max frames to reduce file size
- **File size limit** - enable a target KB cap; the app auto-compresses in multiple passes until the file meets the limit, or uploads the best result it can achieve

### Network
- Scan and connect your device to a different WiFi network
- Scan and connect your PC to a WiFi network
- **WiFi Lock** - keeps your PC connected to a specific network in the background (useful if your PC keeps switching away from the device's network)

### Settings
- Set device IP address
- View firmware version and device storage usage
- Adjust request timeout

---

## Requirements

- Windows 10 or 11
- GeekMagic SmallTV-Ultra on the **same local WiFi network** as your PC
- The device IP address (find it in the official GeekMagic app or your router's device list)

---

## Installation

1. Download the latest `GeekMagic Controller.exe` from the [Releases](../../releases) page
2. Run the `.exe` - no installation needed
3. Enter your device's IP address in **Settings**
4. Start controlling your display

> Settings are saved automatically to `%APPDATA%\GeekMagic Controller\settings.json`

---

## Finding Your Device IP

- Open the official GeekMagic app - the IP is shown on the device info screen
- Or check your router's connected devices list and look for **GIFTV**
- Or look at the display itself - the IP may be shown on the network screen

---

## Tips

- **GIF not working on device?** Use the GIF Compression panel to reduce colors (try 8–16) and frames (try 10–20). The ESP8266 chip has limited memory - simpler GIFs with fewer colors decode more reliably.
- **Enable the file size limit** for weather GIFs - 30–50 KB is a safe target for reliable playback.
- **WiFi Lock** is useful if your PC auto-switches away from the device's network. Set the interval to 10–30 seconds.

---

## Disclaimer

This is an unofficial third-party application. GeekMagic and SmallTV-Ultra are trademarks of their respective owners. This app communicates with the device over its local HTTP API and does not modify any firmware.

