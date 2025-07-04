# Glove Orchestra 🎵🙌

## 🎧 Intro to Sonic Art: Glove Orchestra  

## 🎶 Project Overview  
**Glove Orchestra** is an interactive audiovisual performance system where anyone can become a band performer just by wearing gloves. It integrates sound generation, camera-based interaction, and real-time generative visuals.

---

## 🎹 Key Features

### 1. Random Melody Generator
- Ambient additive synthesis
- 360 BPM tempo
- Generates base melody for the performance

### 2. Camera Launchpad (Requires 2 Laptops)
#### (1) Webcam System
- Built with Jitter (`p.window`, `jit.scissors`)
- Extracts RGB values from webcam
- Detects high red channel intensity to trigger specific toggles
- Sends values to server via `udpsend`

#### (2) Main Server
- Receives input via `udpreceive`
- Plays sound linked to that region or trigger

### 3. Visual Feedback via TouchDesigner
- Real-time generative visuals synchronized to sound
- Uses CHOPS & TOPS (Amplitude + Frequency input)
- Max MSP patcher feeds audio into TouchDesigner
- Enhances immersion with reactive visual aesthetics

---

## 🌈 Artistic Intentions

**Inspired by Loop Station Performances**

**We wanted to create something that transforms simple gestures into full-spectrum audiovisual expression.**

### Goals:
1. Explore the integration of human motion + sound + visual response  
2. Offer a personal immersive art experience  
3. Build community through collaborative creativity and sound play

## 🎥 Demo Video
*Includes live footage of:*
- Melody generation
- Camera-triggered sound activation
- Audio-responsive visual artwork

# Glove Orchestra 🎵🙌

## 🎧 Sonic Art 프로젝트 소개: Glove Orchestra  

## 🎶 프로젝트 개요  
**Glove Orchestra**는 장갑을 착용하기만 하면 누구나 밴드 연주자가 될 수 있는 인터랙티브 오디오·비주얼 퍼포먼스 시스템입니다.  
손의 움직임을 통해 소리를 생성하고, 실시간으로 시각화되는 예술 경험을 제공합니다.

---

## 🎹 주요 기능

### 1. 랜덤 멜로디 생성기
- Ambient Additive Synthesis 기반
- 템포: 360 BPM
- 배경 음악 자동 생성

### 2. 카메라 런치패드 (노트북 2대 필요)
#### (1) 웹캠 시스템 (클라이언트)
- Jitter 라이브러리 사용 (`p.window`, `jit.scissors`)
- 웹캠에서 RGB 값을 추출
- 빨간색(R) 채널 값이 특정 임계값 이상일 때 해당 토글 활성화
- `udpsend`를 통해 메인 서버로 값 전송

#### (2) 메인 서버
- `udpreceive`로 클라이언트 신호 수신
- 해당 위치에 연결된 사운드 재생

### 3. TouchDesigner 시각화
- 소리의 진폭 및 주파수를 기반으로 생성되는 실시간 비주얼 아트
- CHOPS 및 TOPS 사용
- Max MSP patcher와 TouchDesigner를 오디오 입력으로 연동
- 퍼포먼스에 몰입감을 더하는 예술적 시각 효과 구현

---

## 🌈 기획 의도

**Loop Station 공연에서 영감을 받았습니다**

**간단한 손동작이 시각과 청각을 아우르는 표현으로 확장되기를 기대함**

### 목표:
1. 인간의 움직임 + 사운드 생성 + 비주얼 반응의 통합 탐색  
2. 개인의 몰입형 예술 경험 제공  
3. 공동 창작을 통해 커뮤니티 참여 기회 제공

## 🎥 데모 영상
*다음 내용을 포함한 시연 영상:*
- 자동 멜로디 생성
- 카메라 기반 사운드 트리거
- 사운드 시각화 예술
