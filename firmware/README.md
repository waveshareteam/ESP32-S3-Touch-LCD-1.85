# ESP32-S3-Touch-LCD-1.85 Firmware

[简体中文](README_ZH.md)

| File | Purpose |
| --- | --- |
| [`ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin`](ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin) | Tests the onboard functions of the ESP32-S3-Touch-LCD-1.85. |

Connect the board with a USB data cable. Open a terminal in this directory, use esptool 5 or later, and replace `PORT` with the board's serial port.

Erasing the entire flash clears the firmware, settings, and user data. Back up any data you need first.

```sh
python -m esptool --chip esp32s3 --port PORT erase-flash
python -m esptool --chip esp32s3 --port PORT write-flash 0x0 ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin
```

After flashing, reset the board and confirm that the test program starts.
