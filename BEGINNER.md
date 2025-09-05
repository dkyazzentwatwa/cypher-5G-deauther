# Getting Started with Cypher 5G Deauther

Cypher 5G Deauther is an experimental firmware for the BW16 board that demonstrates how Wi-Fi deauthentication attacks work on 2.4 GHz and 5 GHz networks. The project combines custom Wi-Fi packet generation with an OLED display and buttons for an on-device interface.

## Important Safety Notes

- **Educational use only.** Deauthentication can disrupt wireless networks. Operate the device only on networks you own or have explicit permission to test.
- **Follow local laws.** Many regions treat unauthorized interference with communications as illegal. Always research and comply with regulations in your jurisdiction.
- **Limit radio emissions.** Use the lowest power necessary and avoid performing attacks near critical infrastructure.
- **Respect privacy.** Never capture or transmit data beyond what is required for experimentation.

## Repository Overview

- `RTL8720DN_SSD1306_FIX/`: Compatibility layer that patches the Adafruit SSD1306 library so it works with the BW16 board.
- `oled_deauther/`: Main Arduino sketch (`oled_deauther.ino`) and helper code for crafting and sending custom Wi‑Fi frames.
- `img/`: Photos of the assembled device and UI.

## Hardware Requirements

According to the project README, a basic setup includes an SSD1306 display, three buttons, and a BW16 board (the BW16E variant is not supported).

## Uploading and Using the Firmware

1. Copy the contents of `RTL8720DN_SSD1306_FIX` into your Arduino `libraries` folder before compiling so the display will work properly.
2. Open `oled_deauther/oled_deauther.ino` in the Arduino IDE, select the BW16 board, and upload.
3. After booting, use the buttons to navigate or connect to the web UI (default credentials are `littlehakr` / `0123456789`).

## Further Learning

Explore the source files to understand how Wi‑Fi frames are crafted and transmitted. Experiment in a controlled lab environment and document your findings to build good security research habits.

