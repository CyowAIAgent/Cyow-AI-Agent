# CyowGlass
CyowGlass is an AI companion project. Different from traditional AI companions, it uses holographic projection technology and intelligent AI companion system to provide more private and safe role-playing. Users can customize their own AI companions and project them in their own rooms. It allows humans and AI to live together and brings science fiction scenes into reality.

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
- 2D characters: Live2D production (users can find tutorials or use Lily)

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















## Donate
Thank you for your interest in supporting MicroRealEstate. Every contribution will help us pay our ongoing maintenance and development costs 🙏

## Contact
X:


