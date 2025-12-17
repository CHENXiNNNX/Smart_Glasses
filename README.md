<h1 align="center">Smart Glasses</h1>

<p align="center">基于 RV1106 的智能眼镜项目</p>

## 📖 简介

本项目是基于 Rockchip RV1106 开发的智能眼镜系统，集成 AI 对话、AI 识图、音视频实时通信等功能。

**支持平台**: Echo-Mate 开发板

**硬件开源**: 设计中

## 📁 仓库结构

```
Smart_Glasses/
├── Demo/                        # 演示程序
│   └── Smart_Glasses_demo/      # 智能眼镜主程序
│       ├── app/                 # 应用模块
│       │   ├── chatbot/         # AI聊天机器人
│       │   ├── media/           # 音视频处理
│       │   ├── protocol/        # 通信协议（WebRTC/WebSocket/MQTT）
│       │   ├── network/         # 网络管理（WiFi/蓝牙/LTE）
│       │   └── tool/            # 工具库
│       └── test/                # 单元测试
│
└── SDK/                         # 开发SDK
    ├── rv1106-sdk/              # 基于 Luckfox 的 SDK
    └── README.md                # SDK使用说明
```

## 🚀 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/CHENXiNNNX/Smart_Glasses.git
cd Smart_Glasses
git submodule update --init --recursive
git lfs pull
```

### 2. 配置开发环境

推荐使用 **Ubuntu 22.04 LTS**，详见 [SDK/README.md](./SDK/README.md)

### 3. 编译

```bash
cd Demo/Smart_Glasses_demo
mkdir build && cd build
cmake ..
make -j$(nproc)
```

## 🎯 核心功能

| 功能 | 说明 |
|------|------|
| **AI 对话** | 唤醒词检测、语音识别、LLM 对话、TTS 合成 |
| **AI 识图** | 图像分析与理解 |
| **音视频** | 实时采集、编码、WebRTC 传输 |
| **网络通信** | WiFi/蓝牙/LTE 连接管理 |

## 📚 文档

- [SDK 开发环境配置](./SDK/README.md)
- [Demo 使用说明](./Demo/README.md)

## 🔗 致谢

本项目基于 [Echo-Mate](https://github.com/No-Chicken/Echo-Mate.git) 开发
