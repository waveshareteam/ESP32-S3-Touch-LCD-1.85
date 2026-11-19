# ESP32-S3-Touch-LCD-1.85 板载外设测试

[English](README.md) | [简体中文](README_ZH.md)

## 功能

通过 LVGL 显示板载设备状态，并提供触摸操作的音乐播放器和语音控制功能。

## 硬件需求

- ESP32-S3-Touch-LCD-1.85 开发板及 USB 数据线
- 播放音乐还需要兼容扬声器，以及根目录存有 MP3 文件的 microSD 卡

## 怎么运行

在[仓库首页](../../../README_ZH.md)所列的 ESP-IDF 环境中打开此目录并运行：

```bash
idf.py set-target esp32s3 build flash monitor
```

## 预期现象

屏幕显示系统和外设信息，滑动到音乐页面可浏览 microSD 卡中的音乐。说出 “Hi ESP” 可以启动语音识别。

## 常见问题

如果语音识别未启动，请重新编译并烧录完整工程，确保语音模型分区已烧录。如果音乐列表为空，请检查 microSD 卡和文件位置。
