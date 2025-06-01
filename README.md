# LoRa Chat TX Example

This project is an Arduino sketch for a simple LoRa-based chat transmitter and receiver, using the [RadioHead](http://www.airspayce.com/mikem/arduino/RadioHead/) library with an RFM95 LoRa module. It allows you to send and receive text messages wirelessly, making it perfect for experimentation and learning.

---

## ✨ Features

- **Two-way chat** over LoRa.
- **Serial interface** for typing and reading messages.
- **Configurable frequency** and transmit power.
- **Simple and lightweight** sketch for quick testing.

---

## 🔧 Hardware Required

- Arduino-compatible board (e.g., Uno, Nano, Leonardo)
- RFM95 LoRa module (or compatible breakout board)
- Jumper wires

---

## ⚡ Pin Connections

| RFM95 Pin | Arduino Pin  |
|-----------|--------------|
| **CS**    | 8            |
| **RST**   | 4            |
| **INT**   | 7            |
| **MOSI**  | 11 (Uno)     |
| **MISO**  | 12 (Uno)     |
| **SCK**   | 13 (Uno)     |
| **GND**   | GND          |
| **3.3V**  | 3.3V         |

> 💡 **Note:** Some Arduino boards (like Nano) share SPI pins with Uno. Check your board's documentation for exact SPI pinout if you’re using a different board.

---

## 🚀 Getting Started

1. **Connect** the RFM95 module to your Arduino using the pinout table above.
2. **Install the RadioHead library**:  
   - Go to **Sketch** → **Include Library** → **Manage Libraries...**  
   - Search for “RadioHead” and install it.
3. **Open the sketch**:  
   - File → Open → `lora-chat-tx-01.ino`
4. **Select your board and port** in the Arduino IDE.
5. **Upload** the sketch.
6. **Open the Serial Monitor** (set baud rate to `115200`).
7. **Chat!**  
   - Type a message and press Enter to send it via LoRa.  
   - Incoming messages will be displayed in the Serial Monitor.

---

## ⚙️ Configuration

| Parameter        | Default Value   | Description                                   |
|------------------|-----------------|-----------------------------------------------|
| **Frequency**    | 952.2 MHz       | Defined by `RF95_FREQ`. Adjust for your region (e.g., 868 MHz, 915 MHz). |
| **Transmit Power** | 23 dBm        | LoRa transmit power. Configurable in the sketch. |

---

## 📜 License

This project is provided **as-is** for **educational purposes only**. Feel free to modify and adapt it to your needs!

---

## 🙌 Acknowledgments

- [RadioHead Library by AirSpayce](http://www.airspayce.com/mikem/arduino/RadioHead/)

---

Happy chatting! If you have questions or improvements, feel free to reach out. 🚀
