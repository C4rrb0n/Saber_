# Saber Lighting System (WIP)  
An open-source lighting control platform inspired by **Whelen Cencom Core**, designed for construction and roadside work vehicles.

---

## 🚧 Project Status

> **Work in progress.**  
> This system is in early development and evolving rapidly.  
> Architecture, tooling, and firmware are all subject to change.

---

## 🧠 Why This Exists

This project is the result of a lifelong fascination with lighting and control systems.

It started back in high school, where I designed a custom **32×32 LED matrix display** that played arcade-style games like **Tetris**, **Snake**, and **Pong**. I was drawn to the challenge of visual expression through code — how timing, color, and animation could create functional and eye-catching systems.

Now, working in **construction**, I needed effective warning lights for my personal vehicle. That search led me to **Whelen** and their **Cencom Core** system. I quickly became *captivated* by the sophistication and flexibility of their lighting control technology — the way it handles phasing, DVI effects, directional output, and precise behavior mapping. It’s a masterpiece of functional design.

But the cost is significant, and out of reach for personal or small-scale use. So this project is my attempt to **build an accessible alternative** — something powerful, modular, and customizable, yet affordable and open-source. A tool that others in the construction and public works world could also benefit from.

---

## 🧩 Project Scope

**Saber** is a modular, programmable lighting system built from scratch. It aims to replicate — and eventually expand on — the behavior-driven, phase-aware lighting philosophy of commercial-grade systems like Whelen Cencom Core.

---

## 🔧 Core Components

### 🎨 Visual Pattern & Mode Editor

A UI for designing:
- Lighting modes made up of timed rows
- Per-section pattern, color, and phase settings
- Preview playback with timing and phasing

### ⚙️ Lighting Controller

Runs on a **32-bit microcontroller**, handling:
- Pattern playback and timing logic
- Direct and CANBus outputs
- Real-time response to control input

### 💡 Lighting Hardware

Supports:
- **Direct outputs** for simple lights
- **CANBus** networked devices (e.g. visor bars, traffic advisors) with **RGBW LEDs** and per-section control

> RGBW addressable LEDs are only used within networked devices, not driven directly by the controller.

### 🎛️ Control Interface

Support for:
- **Buttons**
- **Slide switches**
- **Indicator LEDs**
- **Backlighting effects**
- **Vehicle signal inputs** (e.g. turn signals, hazards, brakes)  
  These may be supported via digital input lines or by listening to the vehicle's **CANBus** network, depending on vehicle integration.

All control mappings are configurable via the editor.

---

## 📦 Configuration & Export

Outputs a structured configuration that can be deployed to the controller and any connected CANBus devices.  
Supports future reconfiguration without rewriting firmware.

---

## 🧭 Design Goals

- ⚠️ **Roadside safety focus** – for construction and utility vehicles  
- 🧩 **Modular** – supports a wide range of hardware layouts and behaviors  
- 🎚️ **Precision** – per-section phasing and waveform-based intensity control  
- 🧪 **Previewable** – simulate everything in software before deploying  
- 📡 **Scalable** – supports both small vehicles and large multi-light installations  
- 🔓 **Open** – protocols, formats, and tooling are all transparent and customizable  

---

## 📸 Media Coming Soon

- Pattern editor screenshots  
- Example pattern animations  
- Hardware setup previews  

---

## 📜 License

To be determined — an open-source license (e.g., MIT or BSD) will be selected when the project stabilizes.
