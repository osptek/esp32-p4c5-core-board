<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK ESP32-P4C5 核心板</h1>

<p align="center"><b>高性能 RISC-V 双核 · 强大图像多媒体处理 · 小尺寸邮票孔核心板</b></p>

<p align="center"><a href="./README_EN.md">English</a> | 简体中文</p>

<p align="center">
  <img alt="MCU: ESP32-P4" src="https://img.shields.io/badge/MCU-ESP32--P4-E7352C?style=flat-square" />
  <img alt="Wireless: ESP32-C5HF4" src="https://img.shields.io/badge/Wireless-ESP32--C5HF4-0A7BBB?style=flat-square" />
  <img alt="Clock: 360 MHz" src="https://img.shields.io/badge/Clock-360_MHz-F39C12?style=flat-square" />
  <img alt="Flash: 16 MB" src="https://img.shields.io/badge/Flash-16_MB-27AE60?style=flat-square" />
  <img alt="PSRAM: 32 MB" src="https://img.shields.io/badge/PSRAM-32_MB-27AE60?style=flat-square" />
  <img alt="Size: 25x25 mm" src="https://img.shields.io/badge/Size-25x25_mm-6C5CE7?style=flat-square" />
</p>

<p align="center"><img alt="OSPTEK ESP32-P4C5 核心板产品图" src="./images/product.png" width="640" /></p>

## 目录

- [产品简介](#产品简介)
- [产品特性](#产品特性)
- [应用场景](#应用场景)
- [规格参数](#规格参数)
- [硬件资源](#硬件资源)
- [配套底板](#配套底板)
- [仓库结构](#仓库结构)
- [相关资料](#相关资料)
- [购买链接](#购买链接)
- [技术支持](#技术支持)

---

## 产品简介

> 📌 当前参数基于 **ESP32-P4 芯片 v1.3 版本**。

OSPTEK ESP32P4C5 核心板（ESP32-P4C5-Core）是一款基于乐鑫 ESP32-P4 设计的小尺寸
邮票孔核心板，板载 16 MB NOR Flash 与 32 MB PSRAM，并集成 ESP32-C5 芯片，提供
Wi-Fi 6（2.4/5 GHz 双频）与蓝牙 5（LE）无线连接（板载 IPEX 天线接口）。

主控 ESP32-P4 内置 2 个高性能（HP）RISC-V 内核和 1 个低功耗（LP）内核，主频高达 360 MHz；集成 JPEG 编解码器、像素处理加速器（PPA）、H.264 视频编码器、图像信号处理器（ISP）和 MIPI 接口，具备强大的图像与多媒体处理能力。

---

## 产品特性

- ⚡ **高性能双核**：ESP32-P4 双核 RISC-V 处理器，主频高达 360 MHz
- 💾 **大容量存储**：板载 16 MB Flash + 32 MB PSRAM，从容运行大型应用
- 🎨 **强大多媒体**：集成 JPEG 编解码、H.264 视频编码、PPA、ISP、MIPI 接口，胜任图像与视频处理
- 📶 **无线连接**：Wi-Fi 6 + 蓝牙 5（LE），板载 IPEX 天线接口（ESP32-C5）
- 🔌 **全引脚引出**：完整引出 ESP32-P4 引脚，外设资源灵活可用
- 📐 **小巧易集成**：小尺寸邮票孔封装，便于集成到自有底板
- 🛠️ **开发资源完善**：配套中英文文档齐全，基于 ESP-IDF 官方生态开发

---

## 应用场景

- 🏠 智能家居
- 🏭 工业自动化
- 📱 消费电子
- 🖥️ HMI 人机交互
- 🤖 电子机器人
- 📷 摄像头视频流传输
- 🔌 USB 设备

---

## 规格参数

### 主控与存储

| 项目     | 规格                                     |
| -------- | ---------------------------------------- |
| 主控芯片 | 乐鑫 ESP32-P4                            |
| CPU 内核 | RISC-V 32 位双核（HP）+ 单核（LP）        |
| 主频     | HP 系统 360 MHz / LP 系统 40 MHz         |
| ROM      | 128 KB（HP）+ 16 KB（LP）                |
| SRAM     | 768 KB L2MEM（HP）+ 32 KB（LP）          |
| Flash    | 16 MB（板载 NOR Flash）                  |
| PSRAM    | 32 MB（片内叠封）                        |

### 无线

| 项目     | 规格                                        |
| -------- | ------------------------------------------- |
| 无线芯片 | ESP32-C5HF4                                  |
| 无线协议 | Wi-Fi 6（2.4/5 GHz 双频）+ 蓝牙 5（LE）      |
| 天线     | 板载 IPEX-1 天线接口                        |

### 外设接口

| 接口          | 数量 | 接口                     | 数量 |
| ------------- | ---- | ------------------------ | ---- |
| GPIO          | 55   | I2S / LP I2S             | 3 / 1 |
| SPI / LP SPI  | 2 / 1 | USB Serial/JTAG          | 1    |
| UART / LP UART | 5 / 1 | 高速 USB 2.0 OTG         | 1    |
| I2C / LP I2C  | 2 / 1 | 全速 USB 2.0 OTG         | 1    |
| I3C           | 1    | SDIO                     | 1    |
| MIPI CSI-2    | 1    | 100 Mbps 以太网 MAC      | 1    |
| MIPI DSI      | 1    | TWAI（兼容 ISO 11898-1） | 3    |
| PARLIO 并行接口 | 1  | LED PWM / MCPWM          | 1 / 2 |

### 图像与多媒体

- JPEG 编解码器 ×1
- 像素处理加速器（PPA）×1
- 图像信号处理器（ISP）×1
- H.264 视频编码器 ×1

### 模拟与传感

- 12 位多通道 ADC ×2
- 温度传感器 ×1
- 触摸传感器 ×1
- 模拟电压比较器 ×1
- 欠压监测 ×1

### 电气参数

| 项目         | 最小 | 典型 | 最大 | 单位 |
| ------------ | ---- | ---- | ---- | ---- |
| 供电电压 VCC | 3.0  | 3.3  | 3.6  | V    |
| 供电电流     | —    | 1    | —    | A    |
| 工作温度     | -40  | —    | 85   | °C   |

---

## 硬件资源

### 板载资源

| 器件  | 说明                                    |
| ----- | --------------------------------------- |
| 主控  | 乐鑫 ESP32-P4                           |
| 无线  | ESP32-C5HF4（Wi-Fi 6 + 蓝牙 5 LE）      |
| Flash | 16 MB（板载 NOR Flash）                 |
| PSRAM | 32 MB（ESP32-P4 片内叠封）              |
| 天线  | 板载 IPEX-1 天线接口（LAN_OUT）         |
| 封装  | 小尺寸邮票孔，共 88 Pin                 |

### 功能框图

<p align="center"><img alt="ESP32-P4C5 核心板功能框图" src="./images/block-diagram.png" width="620" /></p>

### 引脚图

<p align="center"><img alt="ESP32-P4C5 核心板引脚图" src="./images/pinout.png" width="620" /></p>

### 引脚定义

核心板共 **88 Pin**（邮票孔）。完整引脚定义见 👉 **[引脚定义表](./pages/引脚定义.md)**

### 内部连接（ESP32-C5 ↔ ESP32-P4）

ESP32-C5 与 ESP32-P4 之间通过 **SDIO + IO** 互联通信，连接关系如下：

<p align="center"><img alt="ESP32-C5 与 ESP32-P4 内部连接图" src="./images/c5-p4-connection.png" width="560" /></p>

### 尺寸图

<p align="center"><img alt="ESP32-P4C5 核心板尺寸图" src="./images/dimensions.png" width="640" /></p>

模块尺寸 **25.00 × 25.00 mm**（±0.15 mm）。

### 回流焊温度曲线

<p align="center"><img alt="ESP32-P4C5 核心板回流焊温度曲线" src="./images/reflow-profile.png" width="560" /></p>

> 焊料：锡银铜合金无铅焊料（SAC305）；峰值温度 235–250 ℃，峰值时间 30–70 s。

### 存储条件

| 项目             | 参数                                      |
| ---------------- | ----------------------------------------- |
| 潮湿敏感度（MSL）| 3 级                                      |
| 存储条件         | 密封 MBB 袋中，< 40 ℃ / 90%RH 非冷凝环境   |
| 拆封后使用       | 25 ± 5 ℃ / 60%RH 环境下，168 小时内       |

---

## 配套底板

本核心板的配套开发板为 **ESP32-P4C5-Module 开发板**（`esp32-p4c5-module-dev-board`），
板载 USB、MIPI-CSI / MIPI-DSI 等接口，并将核心板引脚全部引出，方便快速评估与二次开发。

<table align="center">
  <tr>
    <td align="center"><img alt="ESP32-P4C5-Module 开发板正反面" src="./images/dev-board.png" width="360" /></td>
    <td align="center"><img alt="ESP32-P4C5-Module 开发板斜视图" src="./images/dev-board-angle.png" width="360" /></td>
  </tr>
</table>

开发板独立仓库：

- GitHub：<https://github.com/osptek/esp32-p4c5-module-dev-board>
- Gitee：<https://gitee.com/osptek/esp32-p4c5-module-dev-board>

---

## 仓库结构

```
esp32-p4c5-core-board/
├── README.md          # 产品说明（本文档）
├── README_EN.md       # 英文说明
├── docs/              # 数据手册、使用指南等 PDF 资料
├── images/            # README 及文档使用的图片
└── pages/             # 详细子文档
    ├── 引脚定义.md            # 完整 88 Pin 引脚定义表（中文）
    └── pin-definition_EN.md   # 完整 88 Pin 引脚定义表（英文）
```

---

## 相关资料

### 本产品资料

- [ESP32-P4C5-Core 核心板使用指南（中文）](./docs/ESP32-P4C5-Core核心板_使用指南2026.1.6.pdf)
- [ESP32-P4C5-Core Core Board User Guide（英文）](./docs/ESP32-P4C5-Core_User%20Guide%2020260521.pdf)

### 芯片资料（乐鑫官方）

- [ESP32-P4 数据手册 v1.3（中文）](https://documentation.espressif.com/esp32-p4-chip-revision-v1.3_datasheet_cn.html)
- [ESP32-P4 数据手册 v1.3（英文）](https://documentation.espressif.com/esp32-p4-chip-revision-v1.3_datasheet_en.html)
- [ESP32-P4 技术参考手册 v1.3（中文）](https://documentation.espressif.com/esp32-p4-chip-revision-v1.3_technical_reference_manual_cn.pdf)
- [ESP32-P4 技术参考手册 v1.3（英文）](https://documentation.espressif.com/esp32-p4-chip-revision-v1.3_technical_reference_manual_en.pdf)
- [ESP32-P4 产品主页（中文）](https://www.espressif.com/zh-hans/producttype/esp32-p4)
- [ESP32-P4 产品主页（英文）](https://www.espressif.com/en/producttype/esp32-p4)
- [ESP32-C5 数据手册（中文）](https://documentation.espressif.com/esp32-c5_datasheet_cn.html)
- [ESP32-C5 数据手册（英文）](https://documentation.espressif.com/esp32-c5_datasheet_en.html)
- [ESP32-C5 产品主页（中文）](https://www.espressif.com/zh-hans/products/socs/esp32-c5)
- [ESP32-C5 产品主页（英文）](https://www.espressif.com/en/products/socs/esp32-c5)

### 开发指南

- [ESP-IDF 编程指南 · ESP32-P4（中文）](https://docs.espressif.com/projects/esp-idf/zh_CN/latest/esp32p4/index.html)
- [ESP-IDF 编程指南 · ESP32-P4（英文）](https://docs.espressif.com/projects/esp-idf/en/latest/esp32p4/index.html)
- [ESP-IDF 快速入门 · ESP32-P4（中文）](https://docs.espressif.com/projects/esp-idf/zh_CN/latest/esp32p4/get-started/)
- [ESP-IDF 快速入门 · ESP32-P4（英文）](https://docs.espressif.com/projects/esp-idf/en/latest/esp32p4/get-started/)

---

## 购买链接

<p align="center">
  <a href="https://item.taobao.com/item.htm?id=1010716172687"><img alt="淘宝立即购买" src="https://img.shields.io/badge/淘宝-立即购买-FF4400?style=for-the-badge&logo=alibabadotcom&logoColor=white" /></a>
  &nbsp;&nbsp;
  <a href="https://shop110742373.taobao.com/"><img alt="淘宝官方店铺" src="https://img.shields.io/badge/淘宝-官方店铺-FF6A00?style=for-the-badge" /></a>
</p>

<p align="center">
  <a href="https://www.aliexpress.com/item/1005012626312933.html"><img alt="速卖通立即购买" src="https://img.shields.io/badge/速卖通-立即购买-E62E04?style=for-the-badge&logo=aliexpress&logoColor=white" /></a>
  &nbsp;&nbsp;
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="速卖通官方店铺" src="https://img.shields.io/badge/速卖通-官方店铺-FF6A00?style=for-the-badge" /></a>
</p>

**国内（淘宝）**

- 🛒 商品：[OSPTEK ESP32-P4C5 核心板](https://item.taobao.com/item.htm?id=1010716172687)
- 🏬 店铺：[鱼鹰光电工厂店](https://shop110742373.taobao.com/)

**海外（AliExpress）**

- 🌍 商品：[OSPTEK ESP32-P4C5 Core Board](https://www.aliexpress.com/item/1005012626312933.html)
- 🏪 店铺：[OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

---

## 技术支持

如有技术问题或合作需求，欢迎通过以下方式联系我们：

- 📧 技术支持 / 产品咨询：<luyu@osptek.com>
- 🐧 QQ 技术交流群：**985881096**
- 🌐 公司官网：<https://osptek.com/>

---

<p align="center"><sub>© 2026 OSPTEK 鱼鹰光电 · 本仓库资料采用 CC BY 4.0 许可</sub></p>
