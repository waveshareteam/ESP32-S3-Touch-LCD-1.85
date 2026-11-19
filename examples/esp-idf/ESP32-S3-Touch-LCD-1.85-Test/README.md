# ESP32-S3-Touch-LCD-1.85 Peripheral Test

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Uses LVGL to display board status and provides a touch-operated music player and voice control for supported commands.

## Hardware Required

- ESP32-S3-Touch-LCD-1.85 development board and a USB data cable
- For music, a compatible speaker and a microSD card with MP3 files in its root directory

## How to Run

Open this directory in the ESP-IDF environment listed in the [repository README](../../../README.md) and run:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The board displays system and peripheral information. Swipe to the music screen to browse files on the microSD card, or say “Hi ESP” to start voice recognition.

## Troubleshooting

If speech recognition fails to start, rebuild and flash the complete project so the speech model partition is included. If the music list is empty, check the microSD card and file location.
