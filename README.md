# Resource Monitor – Rainmeter Skin

A compact Rainmeter widget that displays real-time CPU and RAM usage in a clean, minimal panel.

---

## Features

- Live CPU usage (percentage + bar).
- Live RAM usage (percentage + bar).
- Lightweight design with translucent rounded panel.
- Smooth text rendering and consistent alignment.
- Fully self-contained skin with zero dependencies.

---

## Preview

<img width="285" height="138" alt="image" src="https://github.com/user-attachments/assets/c8f18d0c-ec65-46f0-8439-26ccfeffa404" />

---

## Installation

1. Download the `.rmskin` file from Releases or clone the repo into your Rainmeter `Skins` directory.
2. Refresh Rainmeter.
3. Load **Resource Monitor** from the Rainmeter manager.

---

## How It Works

The skin uses two built-in Rainmeter measures:

- **CPU**  
  `Measure=CPU`, `Processor=0` → reports total CPU usage.

- **PhysicalMemory**  
  `Measure=PhysicalMemory`, displayed as percentage using `Percentual=1`.

Both are updated on a 1-second cycle (RAM internally every 20 cycles to reduce noise).

---

## Customization (Optional)

All visual parameters such as colors, fonts, sizes, and bar styles are defined in the `[Variables]` section of the skin.  
You may adjust:

- Panel width, height, corner radius  
- Primary font  
- Text sizes and colors  
- Bar colors and bar height  

This is optional; the skin works out-of-the-box with the default theme.
