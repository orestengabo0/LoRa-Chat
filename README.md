# LoRa Chat TX Example

This project is an Arduino sketch for a simple LoRa-based chat transmitter and receiver using the [RadioHead](http://www.airspayce.com/mikem/arduino/RadioHead/) library and an RFM95 LoRa module.

## Features

- Send and receive text messages over LoRa.
- Serial interface for user input and message display.
- Configurable frequency and transmit power.

## Hardware Required

- Arduino-compatible board (e.g., Uno, Nano)
- RFM95 LoRa module
- Jumper wires

### Pin Connections

| RFM95 Pin | Arduino Pin |
| --------- | ----------- |
| CS        | 8           |
| RST       | 4           |
| INT       | 7           |
| MOSI      | 11 (Uno)    |
| MISO      | 12 (Uno)    |
| SCK       | 13 (Uno)    |
| GND       | GND         |
| 3.3V      | 3.3V        |

## Usage

1. Connect the RFM95 module to your Arduino as shown above.
2. Install the [RadioHead](http://www.airspayce.com/mikem/arduino/RadioHead/) library via the Arduino Library Manager.
3. Open `lora-chat-tx-01.ino` in the Arduino IDE.
4. Select your board and port, then upload the sketch.
5. Open the Serial Monitor at 115200 baud.
6. Type a message and press Enter to send it via LoRa.
7. Received messages will be displayed in the Serial Monitor on your pc or testing device.

## Configuration

- **Frequency:** Set by `RF95_FREQ` (default: 952.2 MHz). Adjust as needed for your region and hardware.
- **Transmit Power:** Set to 23 dBm by default.

## License

This project is provided as-is for educational purposes.
