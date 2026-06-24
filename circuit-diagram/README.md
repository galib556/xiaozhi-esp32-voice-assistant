# Circuit Diagram

The wiring diagram below is sourced directly from the **official Xiaozhi AI repository** — I followed this exact diagram for my build.

> **Credit:** [Xiaozhi AI by 78 (虾哥)](https://github.com/78/xiaozhi-esp32) — all credit for the circuit design goes to them and their contributors.

![Official Xiaozhi Wiring Diagram](./wiring2.jpg)

*Source: [https://github.com/78/xiaozhi-esp32/blob/main/docs/v1/wiring2.jpg](https://github.com/78/xiaozhi-esp32/blob/main/docs/v1/wiring2.jpg)*

---

## Pin Mapping (bread-compact-wifi / ESP32-S3)

| Component | Pin | ESP32-S3 GPIO |
|---|---|---|
| INMP441 (Mic) | WS | GPIO 4 |
| INMP441 (Mic) | SCK | GPIO 5 |
| INMP441 (Mic) | SD | GPIO 6 |
| MAX98357A (Amp) | DIN | GPIO 7 |
| MAX98357A (Amp) | BCLK | GPIO 15 |
| MAX98357A (Amp) | LRC | GPIO 16 |
| OLED (SSD1306) | SDA | GPIO 41 |
| OLED (SSD1306) | SCL | GPIO 42 |
