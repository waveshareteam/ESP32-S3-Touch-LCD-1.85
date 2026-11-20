# ESP32-S3-Touch-LCD-1.85 固件

[English](README.md)

| 文件 | 用途 |
| --- | --- |
| [`ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin`](ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin) | 测试 ESP32-S3-Touch-LCD-1.85 的板载功能。 |

使用 USB 数据线连接开发板。在本目录打开终端，使用 esptool 5 或更新版本，将 `PORT` 替换为开发板的串口。

整片擦除 Flash 会清除设备中的固件、设置和用户数据，请提前备份。

```sh
python -m esptool --chip esp32s3 --port PORT erase-flash
python -m esptool --chip esp32s3 --port PORT write-flash 0x0 ESP32-S3-Touch-LCD-1.85_FactoryOnly_20261119.bin
```

烧录完成后复位开发板，确认测试程序正常启动。
