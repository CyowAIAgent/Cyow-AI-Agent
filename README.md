[English](README.md) | [中文](README_zh-CN.md)

# CyowGlass
CyowGlass is an AI companion project. Different from traditional AI companions, it uses holographic projection technology and intelligent AI companion system to provide more private and safe role-playing. Users can customize their own AI companions and project them in their own rooms. It allows humans and AI to live together and brings science fiction scenes into reality.

![88cf26715b98db939e74c1eba61e32a9](https://github.com/user-attachments/assets/66380220-d136-400c-bf22-eeb561830aa7)
![97f70c148d19fa430b1bfc3327f644ec](https://github.com/user-attachments/assets/fd15f848-6e6c-4562-b558-1f39481e85bc)


## Tools
### 1. Hardware
#### 1.1 Projection
- Projection film: electronically controlled atomized film, light transmittance ≥ 92% (to achieve the best projection effect)
- Projection film size: 1.5*2.2m 
- Projector: Epson CH-TW7000
- Projection method: rear projection (the projector is outdoors, the user can design a rain cover and wiring, and the electronically controlled atomized film is attached indoors.)
- Projection requirements: The angle of projection on the window should be adaptable and not affect the indoor living experience.

#### 1.2 Live broadcast
- Camera: SONY ILCE-7M3 FE3.5-5.6/28-70 (ultra-wide angle)
- Computer:
  - ​**CPU**: AMD Ryzen 5 7600X 6-Core Processor (6 Cores)  
  - ​**GPU**: NVIDIA GeForce RTX 4090 (16GB Memory)
- Wireless lavalier microphone: Good Shepherd Lavalier Mic
- Bluetooth speaker: Hanqin USB speaker
- Network: Direct data cable connection

### 2. Software
#### 2.1 Visual
- Client interface: Unity
- 2D characters: Live2D production

#### 2.2 Voice
- ASR: Baidu Voice (API)
- TTS: Fish Audio (API)

#### 2.3 AI model
- Local deployment: Deepseek-LLM-7B-Chat
- Model training method: SFT
- Model training data set source (6000 data):
  - Muxue (Chinese) training set - role play (https://www.modelscope.cn/datasets/Moemuu/Muice-Dataset) Manually modify and review answers for questions (1500 data)
  - Dialogue-Encyclopedia (Chinese) training set (https://www.modelscope.cn/datasets/qiaojiedongfeng/qiaojiedongfeng) Manually modify and review answers for questions (1500 data)
  - Deepseek-V3 official website, manually modify and review multi-round dialogue data sets that meet the requirements through prompt (3000 data)

#### 2.4 Backend environment
- Linux virtual machine: ubuntu 22.04.5
- ragflowv0.15.1-slim
- mysql: 8.0.39
- es: 8.11.3
- redis (valkey): 8
- minio: RELEASE.2023.12.20T01-00-02Z
- docker: 24.0.2
- docker-compose: 2.27.3

## Startup method
- Hardware preparation: The projector and projection film are installed, and the live broadcast environment is deployed.
- Software preparation: Download the entire project file (including Unity project files, backend server code, etc.), and the user downloads the chat model (Deepseek-LLM-7B-Chat)
- Start the backend server: Open the running path A/B project file
- Start the front-end interface: Open the running path A/B.exe run file (If you want to modify the project, you need to install Unityhub, install the Unity editor through unityhub, and open the A/B project file).

## How to use
- Chat mode: wake up word "hello", the user and Lily start a deep and affectionate chat.
- Live mode: wake up word "start live", the user and Lily chat live, Lily can also reply to the live barrage.
  - Live link: Cyow Lily projects the triangular window - Sony camera shoots the triangular window and the user's chat screen - Sony camera connects to the B station live platform through a data cable - the user chats with Lily - the front-end voice broadcasts out.
- Debate mode: wake up word "start debate", the user and Lily and Ray debate on the topic.
- End of use: wake up word "end conversation, bye, bye", the program exits.
- The current program interactive use of speaking Chinese can achieve the best experience effect.
  
![f4e7db3348a34e3a3d7e552e90ec174e](https://github.com/user-attachments/assets/7f1a0425-f62e-4228-a390-f11265964098)
![67ee2426368cafc31c1561dfcf0fb28b](https://github.com/user-attachments/assets/8241ee84-45bc-4d2d-b123-8316cca02c0b)

## Contact
- http://www.htrworld.com/
- Youtube：https://www.youtube.com/@AI-R12


