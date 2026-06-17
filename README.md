<!-- ===================== BANNER ===================== -->
<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0047AB,100:5C3EE8&height=220&section=header&text=Dongseok%20Kim&fontSize=56&fontColor=FF6B35&animation=fadeIn&fontAlignY=38&desc=AI%20%2F%20Computer%20Vision%20%C2%B7%20Embedded%20%2F%20Hardware&descSize=18&descAlignY=60&descColor=0047AB" width="100%">




<!-- ===================== HEADER ===================== -->
<div align="center">


<br/>

<a href="https://0307102bj41-afk.github.io/" target="_blank">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0047AB,100:5C3EE8&height=150&text=🚀%20View%20My%20Portfolio&fontSize=55&fontColor=ffffff&fontAlign=50&fontAlignY=55&width=900&animation=scaleIn" />
</a>

<br/>
<br/>

> CleanCheck · STM32 RC Control · PLC MPS 프로젝트 상세 문서 + 트러블슈팅 포함

</div>

---

## About

딥러닝 컴퓨터 비전과 임베디드 시스템을 함께 다룹니다.<br/>소프트웨어로 해결책을 설계하고 하드웨어로 동작하는 결과물을 완성합니다.

- **AI / CV** — CNN, YOLO, CLIP, SAM, Grad-CAM 기반 멀티모델 시스템 설계
- **Embedded** — STM32 레지스터 레벨 제어, 실시간 펌웨어 구조 설계
- **IoT** — Raspberry Pi + 센서·액추에이터 통합, 하드웨어-소프트웨어 연동

---

## Tech Stack

#### AI / ML
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=yolo&logoColor=black)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)

#### Embedded / Hardware
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![STM32](https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![PLC](https://img.shields.io/badge/PLC-E60012?style=for-the-badge&logo=mitsubishi&logoColor=white)

#### Tools
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

## Projects

### CleanCheck — 딥러닝 기반 생활공간 청결도 자동 진단 시스템 [![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/Kor-JasonKim/DeepLearning_Project)
> 팀 프로젝트 · 딥러닝 / 컴퓨터 비전
>
> 2026 디바이스마트 ICT 융합 프로젝트 공모전 **장려상 수상**

스마트폰·IoT 홈캠으로 실내 환경을 촬영하면 CNN/YOLO/CLIP/SAM 멀티모델 앙상블이
0~100점 청결 점수와 Grad-CAM 히트맵·SAM 오버레이 시각 피드백을 제공하는 시스템.

<table>
<tr>
<td width="58%" valign="top">

| 항목 | 내용 |
|------|------|
| 모델 | ResNet50 · YOLO · OpenAI CLIP · Meta SAM |
| 데이터 | 자체 구축 4,066장 (방 2,756 / 책상 1,310) |
| 성능 (책상) | Accuracy 96.56% · F1 0.9560 · AUC 0.9971 |
| 성능 (방) | Accuracy 95.97% · F1 0.9559 · AUC 0.9917 |
| 하드웨어 | Raspberry Pi 5 + 부저 실시간 알림 연동 |
| 담당 | Keras 모델 설계·학습 · Grad-CAM·CLIP 구현 · Flask 서버 |

**핵심 트러블슈팅** <br/>
- 조명·색상 과의존 오분류(Grayscale 전처리) <br/>
- 과적합(EarlyStopping·Dropout)<br/>
- 데이터 편향(Grad-CAM 기반 데이터 보강)<br/>
- TF 버전 추론 불일치(Linux 환경 일원화)

`Python` `Keras` `YOLO` `CLIP` `SAM` `Grad-CAM` `Flask` `Raspberry Pi`

</td>
<td width="42%" valign="top" align="center">

<img src="https://0307102bj41-afk.github.io/assets/ai_uiux2.png" width="100%" alt="CleanCheck 판독 결과 화면">
<br/>
<sub><b>판독 결과 화면</b> — Grad-CAM 히트맵 · 청결 점수 · CLIP 분석</sub>

</td>
</tr>
</table>

---

### STM32 RC Control — 레지스터 기반 임베디드 제어 시스템 [![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-181717?style=flat-square&logo=github)](https://github.com/0307102bj41-afk/STM32_RCCAR_CONTROLLER)
> 팀 프로젝트 · 임베디드 펌웨어 / 학습형 · 코드리뷰형

STM32F411(Cortex-M4) 기반 조이스틱 컨트롤러 + RC카 구동 펌웨어를
레지스터 레벨에서 end-to-end로 구현한 임베디드 프로젝트.

<table>
<tr>
<td width="58%" valign="top">

| 모듈 | 구현 내용 |
|------|-----------|
| ADC | 2축 조이스틱 12bit 입력 수집 |
| UART | 방향·버튼·체크섬 기반 커스텀 패킷 설계 |
| I2C | 1602 LCD 상태 표시 |
| PWM | 좌우 독립 모터 제어 (직진·회전·정지) |
| 구조 | 상태머신 파서 · 인터럽트 디바운싱 · 타임아웃 예외 처리 |

**핵심 트러블슈팅** <br/>
- ADC 변환 미완료 쓰레기 값(EOC 폴링)<br/>
- I2C LCD 초기화 타이밍 깨짐<br/>
- UART 수신 무한 대기·패킷 깨짐(타임아웃 + 상태머신 파서)

`Embedded C` `STM32F411` `ADC` `UART` `I2C` `PWM` `SysTick` `Timer`

</td>
<td width="42%" valign="top" align="center">

<img src="https://0307102bj41-afk.github.io/assets/racing.gif" width="100%" alt="RC카 주행 장면">
<br/>
<sub><b>RC카 주행</b> — 조이스틱 무선 제어 레이싱</sub>

</td>
</tr>
</table>

---

### PLC MPS 자동화 시스템 — 서보 정밀 위치 제어 & 소재 자동 분류 저장 [![Docs](https://img.shields.io/badge/Docs-Portfolio-000000?style=flat-square&logo=github&logoColor=white)](https://0307102bj41-afk.github.io/plc.html)
> 팀 미니 프로젝트 · 산업 자동화 / PLC 프로그래밍

Mitsubishi PLC(Q03UDV)와 서보 모터를 활용해 금속·비금속 소재를 자동 판별하고
3층 창고에 정밀 위치 제어로 적재·배출하는 MPS 기반 산업 자동화 시스템.

<table>
<tr>
<td width="58%" valign="top">

| 항목 | 내용 |
|------|------|
| CPU | Mitsubishi Q03UDV |
| 소재 판별 | 센서 기반 금속/비금속 자동 분류 |
| 위치 제어 | ABS/INC 서보 제어, AXIS Pointer INC 최적화 |
| 안전 설계 | FLS/RLS B접점 Fail-Safe + SW Limit 이중 구조 |
| HMI | GT Designer3 (GOT 2000), 한/영 다국어 지원 |
| 특이사항 | B접점 인터락으로 기능 충돌 원천 차단 |

**핵심 트러블슈팅** <br/>
- 택타임 레지스터 누적 버그(공정 시작 초기화)<br/>
- 선택/전체 비움 위치 충돌(B접점 인터락)<br/>
- 층별 절대 위치 비효율(AXIS Pointer INC 상대 제어 전환)

`Mitsubishi PLC` `GX Works2` `GT Designer3` `Servo Motor` `QD77MS2` `Ladder` `HMI`

</td>
<td width="42%" valign="top" align="center">

<img src="https://0307102bj41-afk.github.io/assets/plc1.png" width="100%" alt="PLC HMI 서보 조작 화면">
<br/>
<img src="https://0307102bj41-afk.github.io/assets/plc2.png" width="100%" alt="PLC HMI 동작 화면">
<br/>
<sub><b>HMI 작화</b> — 서보 조작 · 동작 모니터링</sub>

</td>
</tr>
</table>

---

## Interests

- Deep Learning & Computer Vision
- Embedded Systems & Real-Time Firmware
- IoT & Hardware-Software Integration
- Industrial Automation & PLC
- System Software

---

## Activity

| 기간 | 내용 |
|------|------|
| 2025.12 – 2026.07 | 대한상공회의소 × 한화로보틱스 · 로보티즈 — AI융합 로봇 SW개발자 2기 |
| 2026 | 디바이스마트 ICT 융합 프로젝트 공모전 **장려상** 수상 — CleanCheck |

---

## Contact

- **E-mail** — 0307102bj41@gmail.com
- **GitHub** — [github.com/0307102bj41-afk](https://github.com/0307102bj41-afk)
- **Portfolio** — [0307102bj41-afk.github.io](https://0307102bj41-afk.github.io/)
