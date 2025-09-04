<h1 align="center">Smart_Glasses</h1>

<br>

## 1. Overview

本仓库是基于RV11系列开发的智能眼镜项目，现目前正在积极开发各项基础功能，包括但不限于智能AI对话，AI识图，音视频实时通信，光波导等功能，其中智能AI功能是在开源项目Echo-Mate (https://github.com/No-Chicken/Echo-Mate.git) 进行对于新功能开发

目前支持开发板:
- luckfox pico ultra w 开发板
- echo-mate 开发板

硬件开源地址：待定(设计中)

## 2. 开发环境

推荐使用`ubuntu22.04 LTS` ，首先拉下整个项目：

```shell
git clone https://github.com/CHENXiNNNX/Smart_Glasses.git
cd Smart_Glasses
git submodule update --init --recursive
```
如果要递归更新所有子模块，请执行：

```shell
git submodule update --remote --merge --recursive
```
由于子仓库有大文件LFS，，请执行：

```shell
git lfs pull
```

SDK开发环境与系统配置详见SDK文件夹中的[README.md](./SDK/README.md).

<br>


## 3. 仓库目录说明

```
Smart_Glasses/
├── Demo/                        # Smart_Glasses开发板的demo
│   ├── Smart_Glasses_demo/      # 智能眼镜
│   └── xxx_demo/                # xxx对应的测试用子demo
├── SDK/                         # SDK文件夹
│   ├── rv1106-sdk/              # 基于luckfox的SDK
│   └── README                   # SDK和开发板使用相关说明
```
