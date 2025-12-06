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

<img width="270" height="123" alt="Screenshot 2025-12-06 205405" src="https://github.com/user-attachments/assets/7a79df59-9fb2-4136-9a95-8381b08d2275" />

---

## How It Works

The skin uses two built-in Rainmeter measures:

- **CPU**  
  `Measure=CPU`, `Processor=0` → reports total CPU usage.

- **PhysicalMemory**  
  `Measure=PhysicalMemory`, displayed as percentage using `Percentual=1`.

Both are updated on a 1-second cycle (RAM internally every 20 cycles to reduce noise).

---

## Performance Cost
The skin is rendered from a single resource_monitor.ini file, keeping overhead minimal.
Persistent desktop operation typically consumes 10–30 MB RAM, depending on the system, and maintains ~0% CPU usage.
The runtime footprint is therefore extremely low and imposes no meaningful load on the system.
---

## Customization (Optional)

All visual parameters such as colors, fonts, sizes, and bar styles are defined in the `[Variables]` section of the skin.  
You may adjust:

- Panel width, height, corner radius  
- Primary font  
- Text sizes and colors  
- Bar colors and bar height  

This is optional; the skin works out-of-the-box with the default theme.
