# Nokia Handshake ESP32 Project 

This project recreates the iconic Nokia startup handshake and ringtone using an **ESP32**, an **OLED SSD1306 display**, and a **passive buzzer**.

---

## Components Used

- ESP32 Dev Board  
- OLED SSD1306 Display (I2C)  
- Passive Buzzer  
- Jumper Wires  
- Breadboard or Soldered Setup  

---

## Pin Connections (ESP32)

| Component  | ESP32 Pin |
|------------|-----------|
| OLED GND   | GND       |
| OLED VCC   | 3V3       |
| OLED SCL   | D22       |
| OLED SDA   | D21       |
| Buzzer (+) | D26       |
| Buzzer (-) | GND       |

![image](https://github.com/user-attachments/assets/e57eec7e-20ad-46e7-8e69-7b5ca4b0acd0)

---

## Libraries Required

Make sure you have these installed in your Arduino IDE:

- `Adafruit_GFX`
- `Adafruit_SSD1306`
- `Wire`

You can install them easily via the Arduino IDE **Library Manager**.

---

## Nokia Tune Credit

The Nokia startup tune was adapted from a project by a **GitHub user** (credit to the original creator — username forgotten, sorry).

---

## How It Works

1. When powered on, the OLED screen displays a Nokia-style welcome or animation.
2. Simultaneously, the buzzer plays the classic Nokia handshake ringtone.
3. It's all perfectly synced for a full nostalgic effect!

---

## Important Note (ESP32 Upload Tip)

Some ESP32 boards **do not have automatic bootloader/reset circuits**.  
When uploading your code, **you might encounter an upload error** (e.g., "Failed to connect to ESP32: Timed out...") if you don't assist the upload manually.

**How to fix it:**

- When you see "Connecting..." in the Arduino IDE terminal, **long-press and hold the "BOOT" button** on your ESP32.
- Keep holding until you see "Writing at..." (indicating that the upload has started), then you can release the BOOT button.
- After uploading, if the code doesn't start automatically, **press the "EN" (Reset) button** once to reboot your ESP32 and run the program.

This is normal behavior for many ESP32 development boards without auto-reset hardware.

---

## License

This project is for educational, hobbyist, and nostalgic purposes only.  
The Nokia logo and ringtone are trademarks of Nokia Corporation.

---

## ✨ Created By

**Edjay**

Feel free to fork, modify, or improve this project! 🚀
