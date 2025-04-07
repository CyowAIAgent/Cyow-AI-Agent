# CyowGlass
CyowGlass是一个AI伴侣项目，与传统的AI伴侣不同，全息投影技术加智能AI伴侣系统，它旨在提供更加私密安全的角色扮演，用户可定制自己的AI伴侣，并投影在自己的房间。让人类和AI住在一起，让科幻场景走进现实。

![88cf26715b98db939e74c1eba61e32a9](https://github.com/user-attachments/assets/66380220-d136-400c-bf22-eeb561830aa7)
![97f70c148d19fa430b1bfc3327f644ec](https://github.com/user-attachments/assets/fd15f848-6e6c-4562-b558-1f39481e85bc)

## 工具
### 1. 硬件
#### 1.1 投影
- 投影膜：电控雾化膜，透光率≥92%（可达到最佳投影效果）
- 投影膜尺寸：1.5*2.2m
- 投影仪：Epson CH-TW7000
- 投影方式：背投（投影仪在室外，用户可设计防雨罩和走线，电控雾化膜贴在室内。）
- 投影要求：投影在窗户上的角度适应，不影响室内居住体验。

#### 1.2 直播
- 相机：SONY ILCE-7M3 FE3.5-5.6/28-70（超广角）
- 电脑：
  - **CPU**:AMD Ryzen 5 7600X 6-Core Processor 内核 6
  - **GPU**:NVIDIA GeForce RTX 4090 内存16G
- 无线领夹麦：好牧人领夹麦
- 蓝牙音箱：汉钦 usb音响
- 网络：数据线直连

### 2. 软件
#### 2.1 视觉
- 客户端界面：Unity
- 二次元角色：Live2D制作

#### 2.2 语音
- ASR：百度语音（API）
- TTS：Fish Audio（API）

#### 2.3 AI模型
- 本地部署：Deepseek-LLM-7B-Chat
- 模型训练方法：SFT
- 模型训练数据集来源（6000条）：
   - 沐雪（中文）训练集-角色扮演（https://www.modelscope.cn/datasets/Moemuu/Muice-Dataset）针对问题人工修 改审核答案（1500条）
   - 对话-百科（中文）训练集（https://www.modelscope.cn/datasets/qiaojiedongfeng/qiaojiedongfeng）针对问题人工修改审核答案（1500条）
- Deepseek-V3官网，通过prompt人工修改审核符合需求的多轮对话数据集（3000条）

#### 2.4 后端环境
- linux虚拟机：ubuntu 22.04.5
- ragflowv0.15.1-slim
- mysql：8.0.39
- es：8.11.3
- redis（valkey）：8
- minio：RELEASE.2023.12.20T01-00-02Z
- docker：24.0.2
- docker-compose：2.27.3

## 启动方法
- 硬件准备：投影仪和投影膜安装完毕，直播环境部署完成。
- 软件准备：下载整个项目文件（包含Unity工程文件、后端服务器代码等），用户自行下载聊天模型（Deepseek-LLM-7B-Chat）
- 启动后端服务器：打开运行路径A/B工程文件
- 启动前端界面：打开运行路径A/B.exe文件（若想要修改项目，需要安装Unityhub，通过unityhub安装Unity编辑器，打开A/B工程文件）。

## 使用方法
- 聊天模式：唤醒词“你好”，用户与lily开始进行深入、深情的聊天。
- 直播模式：唤醒词“开始直播”，用户与lily进行聊天直播，lily同时还可以回复直播弹幕。
  - 直播链路：Cyow Lily投影三角窗——Sony相机拍摄三角窗及用户聊天画面——Sony相机通过数据线接入B站直播平台——用户与lily聊天——前端语音播报出来。
- 辩论模式：唤醒词“开始辩论”，用户与lily、Ray进行话题辩论。
- 使用结束：唤醒词“结束对话、拜拜、再见”，程序退出。
- 当前程序交互使用说中文能达到最佳体验效果。

![f4e7db3348a34e3a3d7e552e90ec174e](https://github.com/user-attachments/assets/7f1a0425-f62e-4228-a390-f11265964098)
![67ee2426368cafc31c1561dfcf0fb28b](https://github.com/user-attachments/assets/8241ee84-45bc-4d2d-b123-8316cca02c0b)
