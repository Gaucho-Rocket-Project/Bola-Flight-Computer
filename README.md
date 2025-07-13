# Bola Flight Computer  
*Lead Engineer: Ethan Scanlon & Jacob Ismael*  

> **Status:** Hardware‐only repository – PCB design files, footprints and production data for the first-generation Bola flight computer. Firmware lives in the separate [`bola`](https://github.com/Gaucho-Rocket-Project/bola) repo.

## Overview
Bola is an open-source, miniature flight computer for experimental rockets.  
It is built around an **ESP32-S3** microcontroller and pairs a 9-DoF IMU with a high-resolution barometer to provide real-time state estimation, data-logging and telemetry in a single, compact PCB.  

The hardware in this repository powers the Gaucho Rocket Project’s “Bola” launch vehicle and is released to help other student teams accelerate their avionics development.

## Key Features
| Sub-system | Parts/Notes |
|------------|-------------|
| MCU | Espressif **ESP32-S3** module, 240 MHz dual-core, Wi-Fi & Bluetooth LE|
| Inertial sensing | **ICM-20948** 9-axis IMU (gyro + accel + mag) |
| Altimetry | **BMP581** absolute barometer (32-bit FIFO, 5 Pa RMS) |
| Power | 2-stage regulation: **LD1117-5 V** & **SPX3819-3 V3** LDOs |
| Pyro outputs | Low-side MOSFETs (**DMN3023L-7**) for ejection charges |
| User feedback | JST-XH debug header |
| Connectors | **XT30UPB** main supply; screw terminals for igniters |
| Form factor | 4-layer, 50 × 80 mm PCB < 15 g bare |

## Schematic
![Schematic](https://github.com/user-attachments/assets/9a484144-c24b-4605-bac4-c39f88615eeb)

## PCB Layout
<img width="949" height="752" alt="pcb" src="https://github.com/user-attachments/assets/1d0ce3a2-1f3d-47a9-81b1-a0cfb6a90b0c" />
