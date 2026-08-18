# Phase 1 — IoT & Embedded

![Status](https://img.shields.io/badge/status-complete-2D6CDF)
![Skills](https://img.shields.io/badge/skills-ESP32_·_MQTT_·_Python-16243B)

> First connected devices and real-time control loops — the closed software-to-hardware loop the whole platform is built on.

## Goal

Bring physical devices online and prove the core interaction pattern of the system: software issues a command → hardware acts → hardware reports its real state back.

## What it demonstrates

- **Embedded firmware** on the **ESP32** microcontroller (C++/Arduino)
- **MQTT** publish/subscribe messaging with a **Mosquitto** broker
- **Python control software** driving devices over the network (`paho-mqtt`)
- **Command/state architecture** — separating desired state from actual state
- **Networking** — device-to-broker communication over Wi-Fi (WSL2 networking)

## Key concept

Every device is designed as a **closed feedback loop** — desired state out, actual state back. Separating *intent* from *reality* makes the system observable and reliable, and mirrors the setpoint-vs-measured logic used in control systems. This pattern is reused by every later capability.

## Tech stack

`ESP32` · `C++ / Arduino` · `MQTT` · `Mosquitto` · `Python` · `paho-mqtt` · `Wi-Fi networking`

## Status

**Complete.** Building the first device (MQTT smart lighting) and its control loop. Code and a demo clip will be added here as it's completed.
