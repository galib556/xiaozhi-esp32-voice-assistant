# Circuit Diagram

The wiring diagram below is sourced directly from the **official Xiaozhi AI repository** — I followed this exact diagram for my build.

> **Credit:** [Xiaozhi AI by 78 (虾哥)](https://github.com/78/xiaozhi-esp32) — all credit for the circuit design goes to them and their contributors.

![Official Xiaozhi Wiring Diagram](./wiring2.jpg)

*Source: [https://github.com/78/xiaozhi-esp32/blob/main/docs/v1/wiring2.jpg](https://github.com/78/xiaozhi-esp32/blob/main/docs/v1/wiring2.jpg)*

---

## My Pin Mapping

Fill this in with your actual wiring once confirmed — useful for anyone trying to copy the exact build:

| Component | Pin | ESP32-S3 GPIO |
|---|---|---|
| INMP441 (Mic) | SCK | |
| INMP441 (Mic) | WS | |
| INMP441 (Mic) | SD | |
| MAX98357A (Amp) | BCLK | |
| MAX98357A (Amp) | LRC | |
| MAX98357A (Amp) | DIN | |
| OLED (SSD1306) | SDA | |
| OLED (SSD1306) | SCL | |

---

For the most up-to-date version of the circuit diagram, always refer to the [official Xiaozhi AI repo](https://github.com/78/xiaozhi-esp32/tree/main/docs) directly, as they update it across firmware versions.
