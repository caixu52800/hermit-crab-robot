# hermit-crab-robot
Bionic hermit-crab-shaped AI companion robot (ESP32-S3 N16R8)
# Hermit Crab Robot 寄居蟹机器人

A bionic hermit-crab-shaped AI companion robot built on the ESP32-S3.

## Features

- **Bionic hermit crab body**: 9 servos - 4 legs, 2 claws (2 servos each), 1 eye-stalk - driven by a PCA9685 over I2C
- **Face recognition**: OV2640 camera, with face + voiceprint binding on a self-hosted server
- **Dual-mic array**: voice interaction and sound-source localization
- **MPU6050 IMU**: gait, balance and stuck detection
- **Local wake-up**: ESP-SR WakeNet (wake word requested)
- **Real-time cloud brain**: Doubao real-time end-to-end voice API (ASR / LLM / TTS)
- **Self-hosted server**: dialog, preferences, OTA updates, device-status dashboard
- Offline WakeNet wake-up -> cloud real-time dialog -> physical motions (wave, walk, dance)

## Hardware

- Board: Freenove ESP32-S3 WROOM (16 MB flash, 8 MB octal PSRAM)
- Framework: ESP-IDF v5.5.5 + esp-sr v2.2.2
- Servo driver: PCA9685 (I2C), independent 5-6 V power supply
- Sensors: MPU6050 (I2C), OV2640 camera, dual I2S microphones

## Status

This project is being prepared for commercial sale. A wake word matching the robot's name ("你好小蟹" / "Hello, Little Crab") has been requested from the Espressif community.
