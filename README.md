#  HBS Core

&zwnj;**鸿蒙直播开源内核 |  Open Harmony Broadcaster Software core**&zwnj;

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg){target="_blank"}](https://www.apache.org/licenses/LICENSE-2.0)
[![HarmonyOS](https://img.shields.io/badge/HarmonyOSPC-6.1%2B-orange){target="_blank"}](https://developer.harmonyos.com)
[![Platform](https://img.shields.io/badge/Platform-OpenHarmony-green){target="_blank"}](https://www.openharmony.cn)

---

## 📖 项目简介

HBS Live Core 是一个专为&zwnj;**鸿蒙（HarmonyOS / OpenHarmony）**&zwnj;生态打造的轻量级直播开源内核，提供直播启动、音视频采集、硬件设备连接等核心基础能力接口。内核聚焦于底层能力抽象，不携带任何业务层封控逻辑、域名黑白名单策略或账号鉴权模块，开发者可在此基础上自由构建上层应用。

---

## ✨ 核心特性

- &zwnj;**直播启动引擎**&zwnj; —— 封装推流初始化、编码参数配置、会话管理等核心流程，提供简洁的启动接口
- &zwnj;**硬件连接抽象层**&zwnj; —— 统一摄像头、麦克风、外接采集卡等硬件设备的接入与生命周期管理
- &zwnj;**模块化架构**&zwnj; —— 各功能模块独立解耦，可按需裁剪组合，适配不同产品形态
- &zwnj;**鸿蒙原生适配**&zwnj; —— 深度兼容 OpenHarmony 与 HarmonyOS，充分发挥分布式软总线等系统能力
- &zwnj;**轻量高性能**&zwnj; —— 最小化运行时开销，适用于嵌入式设备、手机、平板等多形态终端

---

## 🏗️ 架构概览

┌─────────────────────────────────────┐
│ 上层应用（闭源/开源） │
├─────────────────────────────────────┤
│ HBS Live Core (Apache 2.0) │
├──────────┬──────────┬───────────────┤
│ 直播引擎 │ 音频模块 │ 视频模块 │
├──────────┼──────────┼───────────────┤
│ 硬件抽象层 (HAL) │
├─────────────────────────────────────┤
│ HarmonyOS / OpenHarmony 系统层 │
└─────────────────────────────────────┘


---

## 📦 模块说明

| 模块 | 功能 | 接口文件 |
|------|------|----------|
| `live-engine` | 推流初始化与生命周期管理 | `include/live_core.h` |
| `audio-hal` | 音频采集设备抽象接口 | `include/audio_device.h` |
| `video-hal` | 视频采集设备抽象接口 | `include/video_device.h` |
| `stream-output` | 编码流输出管道 | `include/stream_output.h` |
| `device-manager` | 硬件设备统一管理 | `include/device_manager.h` |
| `media-codec` | 音视频编码接口封装 | `include/media_codec.h` |

---

## 🚀 快速开始

### 环境要求

- DevEco Studio 5.0 或更高版本
- HarmonyOS SDK API Level 12+
- 目标设备：HarmonyOS / OpenHarmony 设备

### 集成方式

```bash
# 拉取代码
git clone https://github.com/your-org/hbs-live-core.git

# 将内核模块添加到你的项目
ohpm install hbs-live-core


```bash
# 拉取代码
git clone https://github.com/your-org/hbs-live-core.git

# 将内核模块添加到你的项目
ohpm install hbs-live-core
```
---
## 📄 开源协议

本项目遵循 ‌Apache License 2.0‌ 开源协议。

✅ 允许商业使用与闭源衍生作品

✅ 允许修改代码后闭源发布

✅ 提供明确专利授权，保护贡献者权益

⚠️ 分发需保留原始版权声明与许可文件

---

## 🤝 参与贡献

欢迎提交 Issue 与 Pull Request。在提交代码前，请阅读 CONTRIBUTING.md 了解开发规范与提交流程。

---

## 🔗 相关资源

API 接口文档（）

---

## 📧 联系方式
如有技术问题或合作需求，欢迎通过以下方式联系：
#### 邮箱：
                 qq群：903163291
                 linzk1220.gmail.com
                 1701937807@qq.com

---
## 其他仓库地址：
     gitee：https://gitee.com/chomoa/open-harmony-broadcaster-software-core
     GitHub：https://github.com/chomoa/Open-harmony-Broadcaster-Software-Core
     gitcode：https://gitcode.com/youcanyoudone/Open-Harmony-Broadcaster-Software-Core