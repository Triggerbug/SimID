- Then go to **Tools > Board > Board Manager**
- Search and install **esp32** by Espressif Systems

### 3. Install Required Libraries
- Open **Library Manager** (`Sketch > Include Library > Manage Libraries`)
- Install:
- **GxEPD2** (for e‑ink display)
- **Adafruit GFX** (used by GxEPD2)
- **WiFi** (built-in for ESP32)
- Any library recommended by your specific display manufacturer (e.g. Waveshare)

---

## 🔌 Wiring the Display

Coming soon: diagrams in `/hardware/wiring-diagram.png`

Basic guidance (for SPI displays):
| E‑ink Pin | Connects to ESP32 |
|-----------|-------------------|
| VCC       | 3.3V              |
| GND       | GND               |
| DIN (MOSI)| GPIO 23           |
| CLK       | GPIO 18           |
| CS        | GPIO 5            |
| DC        | GPIO 17           |
| RST       | GPIO 16           |
| BUSY      | GPIO 4            |

⚠️ Double-check pin mapping with your display module.

---

## 🚀 Flash the Firmware

- Open the example sketch in `/firmware/`
- Connect the ESP32 via USB
- In Arduino IDE:
- Select the correct board (e.g. **ESP32 Dev Module**)
- Choose the correct COM port
- Click **Upload**

You should see the e‑ink screen refresh and display your first simulated patient data!

---

## 📱 Future Updates

Planned features:
- Wireless data updates via phone (Bluetooth or Wi-Fi)
- Dynamic QR code generation
- Battery life optimization
- 3D printable case files

---

## 💬 Need Help?

If you hit any issues, [open an issue](https://github.com/yourusername/SimID/issues) or post a discussion in the GitHub repo. Collaboration is welcome!

---

## 🔐 Licensing

© 2025 Katherine Rogers – All rights reserved
