# Xiaozhi AI Voice Assistant — ESP32-S3 Build

This is a small hardware project I put together while exploring embedded systems and AI — a working voice assistant built on the ESP32-S3, following the open-source **Xiaozhi AI** project.

I'm a CSE undergrad and this was mostly a "let's see if I can actually get this working" project. No PCB, no enclosure, just a breadboard, a bunch of jumper wires, and a lot of patience.

This repo is **not** my own firmware — I followed Xiaozhi AI's official circuit diagram and flashed their existing firmware. What's here is my documentation of the build: the hardware I used, how I wired it, what I learned, and a demo video of it actually working.

---

## Demo

Video of it introducing itself and explaining what it can do, recorded right after I got everything wired up and flashed.

📁 Check [`video/`](./video) for the clip (or the link I'll drop there once it's uploaded).

---

## Hardware

| Component | What it does here |
|---|---|
| ESP32-S3 | Runs the Xiaozhi firmware |
| MAX98357A | I2S amp, drives the speaker |
| 8Ω 3W speaker | Output |
| INMP441 | I2S mic, picks up voice input |
| 0.96" OLED (SSD1306) | Shows status/face |
| Breadboard + jumper wires | Holding it all together (barely) |

---

## Circuit Diagram

I followed the official diagram from the Xiaozhi AI repo rather than redrawing my own — didn't want to risk introducing an error by copying it by hand. Find it here:

➡️ Official repo: https://github.com/78/xiaozhi-esp32
➡️ Wiring/hardware docs: https://github.com/78/xiaozhi-esp32/tree/main/docs

I've added my own pin mapping notes in [`circuit-diagram/`](./circuit-diagram) for anyone trying to reproduce this exact build.

---

## Credit

All credit for the actual AI/firmware goes to **Xiaozhi AI**, built by [78 (虾哥)](https://github.com/78) and contributors:

🔗 https://github.com/78/xiaozhi-esp32

I didn't write any of the firmware — this repo is just me documenting my own hardware build using their open-source project. If you're interested in the software side, go check out and star their repo, that's where the real work is.

---

## What I learned

- Wiring up I2S devices (mic + amp) on the same ESP32-S3 and getting the timing/clock lines right
- How fragile breadboard audio circuits can be — noise and power issues showed up more than I expected
- Basics of driving an SSD1306 OLED over I2C
- Just generally how satisfying it is when a pile of wires actually starts talking back

---

## Next steps

- [ ] Move off the breadboard onto something more permanent (perfboard at least)
- [ ] Maybe a basic 3D printed case
- [ ] Try customizing the wake word
- [ ] Write up the flashing process in more detail for `docs/`

---

## About me

Undergrad CSE student, learning embedded systems and AI hands-on. Always happy to connect with people working on similar stuff.

---

## License

The build notes, photos, and video in this repo are just personal documentation. The actual Xiaozhi AI firmware has its own license — check the [original repo](https://github.com/78/xiaozhi-esp32) for that.
