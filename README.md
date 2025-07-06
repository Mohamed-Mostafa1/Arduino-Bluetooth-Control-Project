# Arduino Bluetooth Control Project

This project is an Arduino-based Bluetooth control system using the `blue.ino` sketch. It allows you to wirelessly control hardware components (like LEDs, motors, etc.) via a Bluetooth module connected to your Arduino board.

## 🧰 Features

- Wireless communication via HC-05 or HC-06 Bluetooth module
- Serial command reception from a mobile app or PC
- Control of digital outputs (e.g., LED ON/OFF, motor control)
- Compatible with Android serial Bluetooth terminal apps

## 🔌 Hardware Requirements

- Arduino Uno / Mega / Nano
- HC-05 or HC-06 Bluetooth module
- Jumper wires
- Breadboard (optional)
- Components to control (LEDs, motors, relays, etc.)

## 💻 Software Requirements

- Arduino IDE
- Bluetooth Serial Terminal App (like [Serial Bluetooth Terminal](https://play.google.com/store/apps/details?id=de.kai_morich.serial_bluetooth_terminal))

## 🔧 Wiring

| HC-05 Pin | Arduino Pin |
|-----------|-------------|
| VCC       | 5V          |
| GND       | GND         |
| TXD       | RX (D0)\*   |
| RXD       | TX (D1)\*   |

> ⚠️ *Note: It's recommended to use a voltage divider on TX → RX line or use SoftwareSerial on other pins (e.g., D10/D11).*

## 🚀 How to Use

1. Open the `blue.ino` file in Arduino IDE.
2. Upload the sketch to your Arduino board.
3. Pair your Bluetooth module with your mobile phone.
4. Open a Bluetooth terminal app and connect to the module.
5. Send predefined commands (like `1` to turn on an LED, `0` to turn it off).

## 📂 File Description

- `blue.ino`: The main Arduino sketch containing Bluetooth communication logic.

## 📱 Example Commands

| Command | Action         |
|---------|----------------|
| `1`     | Turn LED ON     |
| `0`     | Turn LED OFF    |

> You can customize the commands in the code for different actions.


