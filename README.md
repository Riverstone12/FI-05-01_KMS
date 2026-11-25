# 👋 파형과 타이밍 리포트에서 회로의 동작을 확인하는 엔지니어 강민석입니다.

## 🚀 About Me

- 🎯 **관심 분야** : RTL & FPGA Design, SoC 검증, Physical Design, DFT
- 🔧 **경험 분야** : Verilog RTL 설계, FPGA 실보드 디버깅, SystemVerilog 기반 검증, 28nm ASIC 구현

## 🎓 학력

- **광운대학교 전자공학과** (본전공)
- **광운대학교 인공지능반도체공학** (연계전공)
- **학점** : 3.79 / 4.5
- **재학 기간** : 2019.03 ~ 2025.02 졸업

## 🛠️ Skill

- **Languages**  
  ![Verilog](https://img.shields.io/badge/Verilog-24547A?style=flat-square) ![SystemVerilog](https://img.shields.io/badge/SystemVerilog-345B90?style=flat-square) ![Tcl](https://img.shields.io/badge/Tcl-79529C?style=flat-square) ![C](https://img.shields.io/badge/C-375A7F?style=flat-square) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square) ![MATLAB](https://img.shields.io/badge/MATLAB-C45B28?style=flat-square)
- **EDA & Circuit Tools**  
  ![Vivado](https://img.shields.io/badge/Vivado-C32632?style=flat-square) ![VCS](https://img.shields.io/badge/VCS-594382?style=flat-square) ![Design Compiler](https://img.shields.io/badge/Design%20Compiler-594382?style=flat-square) ![Formality](https://img.shields.io/badge/Formality-594382?style=flat-square) ![PrimeTime](https://img.shields.io/badge/PrimeTime-594382?style=flat-square) ![Innovus](https://img.shields.io/badge/Innovus-9F242B?style=flat-square) ![TestMAX](https://img.shields.io/badge/TestMAX-594382?style=flat-square) ![TetraMAX](https://img.shields.io/badge/TetraMAX-594382?style=flat-square) ![Tessent](https://img.shields.io/badge/Tessent-007D77?style=flat-square)
- **Hardware Platforms**  
  ![Zynq-7015](https://img.shields.io/badge/Zynq--7015-B82E36?style=flat-square) ![TOPST VCP-G](https://img.shields.io/badge/TOPST%20VCP--G-235C91?style=flat-square) ![TOPST D3-G 4GB](https://img.shields.io/badge/TOPST%20D3--G%204GB-235C91?style=flat-square) ![TOPST AI-G](https://img.shields.io/badge/TOPST%20AI--G-235C91?style=flat-square)
- **Operating Systems**  
  ![Linux](https://img.shields.io/badge/Linux-555555?style=flat-square) ![FreeRTOS](https://img.shields.io/badge/FreeRTOS-388044?style=flat-square)

## 🥇 수상

### 한국반도체아카데미 원장상

- **주제** : Samsung 28nm Low-Power 공정 기반 ARM, RISC-V Ibex, Counter 통합 설계
- **주관 / 과정 기간** : 한국반도체아카데미 | 2026.06.22 ~ 2026.08.28
- **활동 내용**
  - **RTL 설계 및 통합** : Counter RTL을 작성하고 ARM, Ibex와 Top에 통합한 뒤 합성 방식에 따른 타이밍 리포트 비교
  - **클록 핀 배치 개선** : 배치 결과에서 클록 핀과 관련 회로 사이의 거리를 확인하고 핀 위치를 조정해 `clk_sys` skew를 30 ps에서 6 ps로 감소
  - **팀 설계 결과** : 코어 크기 5개 조건의 배치 밀도를 비교해 구현 조건을 선정하고, 최종 칩 면적을 기준 설계 대비 약 47.6% 축소

## 💻 경험 / 교육

### 한국팹리스산업협회(KFIA) 팹리스 점프업 일경험 프로그램 5기

- **기간** : 2026.11 ~ 진행 중
- **사용 환경** : FreeRTOS, Linux
- **실습 보드**
  - TOPST VCP-G (`TBM7045EF-XXB-AC`)
  - TOPST D3-G 4GB (`TBC8050BB-XXB-AC`)
  - TOPST AI-G (`TBN7501AA-XXA-AC`)
- **SPI 디버깅** : MAX7219 LED 매트릭스를 연결하고, 칩 선택(GPSB_CsActivate), 데이터 전송(GPSB_Xfer), 칩 선택 해제(GPSB_CsDeactivate) 순서로 호출해 표시 데이터를 전송
- **보드 설정 확인** : PWM 선택 레지스터와 GPIO A10~A13의 핀 기능을 대조해 출력 채널을 확인. CAN 실습에서는 ID 0x0104에 데이터 0x4F를 전송하고 채널 및 비트마스크 로그를 점검
- **빌드 문제 해결** : 소스를 수정해도 보드 동작이 바뀌지 않아 빌드 대상을 추적. 수정한 freertos-vcp와 실제 빌드한 zonal-vcp의 경로 차이를 찾아 변경 사항을 반영

### 한국반도체아카데미 반도체 DFT 전문가 양성과정

- **기간** : 2026.09 ~ 2026.11.13 (240시간)
- **사용 툴** : TestMAX, DFTMAX, TetraMAX, Siemens Tessent
- **Scan 및 ATPG** : Top-down과 Bottom-up 방식으로 Scan을 삽입하고 삽입 전후의 DFT DRC를 점검. Scan Compression 적용 후 TetraMAX로 패턴을 생성하고 검출 여부에 따른 결함 분류와 커버리지를 확인
- **메모리 테스트** : Tessent로 MBIST 회로를 삽입한 뒤 테스트 패턴과 테스트벤치를 생성해 시뮬레이션. March 알고리즘의 메모리 검사 순서와 BIRA/BISR의 결함 분석 및 수리 구조 학습
- **계층형 테스트** : IEEE 1687 IJTAG의 SIB와 TDR 연결을 따라 ICL을 추출하고 PDL을 리타기팅. Graybox를 이용한 코어 외부 테스트와 SSN 패킷의 코어별 대역폭 배분 방식 학습

### 한국반도체아카데미 파운드리향 반도체 Design 전문가 양성과정

- **기간** : 2026.06.22 ~ 2026.08.28 (300시간)
- **사용 툴** : VCS, Design Compiler, Formality, Innovus, PrimeTime
- **논리 구현** : VCS로 RTL을 시뮬레이션한 뒤 Design Compiler로 합성. 합성, Scan 삽입, P&R, ECO로 넷리스트가 바뀔 때마다 Formality로 전후의 논리 등가성을 확인
- **물리 구현** : Innovus에서 Floorplan, 전원망 구성, Placement, CTS, Routing을 수행. 배선 후 기생 성분을 반영해 PrimeTime에서 4개 코너와 2개 모드(Function/Scan)의 타이밍을 분석
- **ECO** : PrimeTime이 생성한 수정 목록을 Innovus에 적용하고 다시 타이밍을 분석. Setup/Hold 조건을 만족하는 범위에서 셀의 문턱전압 종류를 바꿔 누설전력의 변화를 비교

### 한국반도체아카데미 공정 시뮬레이터를 활용한 AI 반도체 공정 설계 교육

- **기간** : 2026.05.29 ~ 2026.06.12 (60시간)
- **사용 툴** : SEMulator3D
- **소자 및 공정** : 소자 물리와 설계 규칙을 학습한 뒤 SEMulator3D의 FinFET 예제를 실행
- **구조 확인** : 공정 순서에 따라 중간 단계의 3D 구조를 비교하며 각 단위 공정이 최종 소자 형상에 어떻게 반영되는지 확인

### 한국반도체아카데미 반도체 검증(DV) 전문가 양성과정

- **기간** : 2026.04.07 ~ 2026.05.20 (180시간)
- **사용 환경** : SystemVerilog, Linux
- **테스트벤치 구성** : Linux 환경에서 SystemVerilog로 제약 기반 입력을 생성하고, Scoreboard로 읽기 결과와 기대값을 비교
- **프로토콜 검증** : 정상 전송, 대기 상태, 오류 응답에서 신호가 변하는 순서를 Checker와 SVA로 검사. Covergroup을 정의해 각 조건이 실제 시뮬레이션에서 실행됐는지 확인

### 한국반도체아카데미 반도체 RTL 설계 전문가 양성과정

- **기간** : 2026.02.23 ~ 2026.04.06 (180시간)
- **사용 환경** : Verilog HDL, Vivado, Zynq-7015
- **RTL 설계** : AMBA 기반 IP를 실습하고, 외부 ADC 데이터시트의 명령 비트와 송수신 타이밍을 Verilog 제어 로직으로 구현
- **FPGA 실습** : Zynq-7015에 설계를 올린 뒤 Vivado ILA로 칩 선택 신호, 수신 카운터, 데이터 유효 신호를 관측해 시뮬레이션에서 의도한 동작과 비교

### 한국반도체아카데미 반도체 설계 개론 (Verilog HDL)

- **기간** : 2026.02.02 ~ 2026.02.13 (60시간)
- **사용 언어** : Verilog HDL
- **제어 로직 설계** : 동작 절차를 Flowchart로 정리한 뒤 상태, 전이 조건, 상태별 출력을 나누어 Moore FSM을 Verilog로 구현
- **IP 분석** : 예제 IP의 모듈 연결과 입력에서 출력까지의 신호 흐름을 따라가며 RTL 구조 분석

### 렛유인에듀 실무 데이터 기반 반도체 소자/공정 엔지니어 융합과정

- **기간** : 2025.02.04 ~ 2025.05.21 (455시간)
- **사용 환경** : Python, Isolation Forest, Random Forest
- **공정 실습** : 반도체 8대 공정과 소자 물리를 학습하고 XR 시뮬레이션으로 단위 공정의 동작 순서를 확인
- **이상 후보 탐색** : 웨이퍼 좌표별 데이터를 정리하고 Isolation Forest의 이상치 비율 설정을 0.05에서 0.035로 조정해 검출 후보의 분포를 비교
- **수율 분석** : 전기적 특성 데이터(Vth, Idsat, Idoff)와 BIN2 수율 데이터를 병합. Random Forest 분류 및 회귀 모델로 수율과 관련된 변수의 중요도를 비교

## 📂 프로젝트

### 28nm ASIC RTL-to-GDS 구현

- **기간 / 환경** : 2026.06 ~ 2026.08 | Samsung 28nm LP, Design Compiler, Formality, Innovus, PrimeTime
- **담당** : 2~8비트 Counter RTL을 작성하고 32비트 ARM 및 RISC-V Ibex와 Top에 통합. 세 블록에 독립 클록을 구성하고, 동일한 목표 주파수에서 논리 합성과 물리 합성의 결과를 비교
- **코어 크기 선정** : 정사각형 코어 5종을 시험 배치. 187.2 × 187.2 µm에서는 배치 밀도가 76.61%였고, 이후 배선과 ECO에 쓸 공간을 확보하기 위해 밀도 68.29%인 198.9 × 198.9 µm를 선택
- **클록 배치 개선** : 배치도에서 클록 핀과 관련 회로가 멀리 떨어진 것을 확인해 핀 위치를 조정. 변경 전후 리포트에서 `clk_sys` skew가 **30 ps → 6 ps**로 감소한 것을 확인
- **테스트 결과** : Scan 압축 적용 전후 체인 수는 6개에서 72개로, 평균 체인 길이는 560에서 43으로 변화. ATPG 결과에서 Test Coverage **99.11%**, Fault Coverage **98.73%** 확인

**팀 최종 설계와 기준 설계 비교**

| 항목 | 기준 설계 | 팀 최종 설계 |
| --- | ---: | ---: |
| Counter 동작 주파수 | 400 MHz | 1 GHz |
| ARM / Ibex 동작 주파수 | 각각 200 MHz | 각각 250 MHz |
| 칩 가로 × 세로 | 330 × 330 µm | 238.9 × 238.9 µm (면적 47.6% 감소) |
| 최종 배치 밀도 | 35.59% | 70.44% |
| 동적 전력 (Function 모드, wcl 코너) | 1.352 mW | 1.928 mW |
| 셀 누설전력 (동일 조건) | 0.6611 µW | 0.5715 µW |

### AMBA APB3 프로토콜 검증

- **기간 / 환경** : 2026.04 ~ 2026.05 | SystemVerilog, SVA, Linux
- **데이터 검증** : 쓰기 트랜잭션에서 기대값을 Scoreboard에 기록하고, 같은 주소의 읽기 트랜잭션이 완료되면 슬레이브 응답과 비교
- **타이밍 검증** : `PREADY`가 늦어져 대기 상태가 이어질 때 주소와 제어 신호가 유지되는지 SVA로 검사. `PSLVERR` 오류 응답, 응답 타임아웃, 리셋 조건을 별도 시나리오로 점검
- **결과** : 제약 기반 입력과 오류 시나리오를 실행하고 Covergroup에서 **프로젝트에 정의한 기능 커버리지 100%** 달성

### FPGA 기반 SPI Master 설계 및 조도 측정

- **기간 / 환경** : 2026.02 ~ 2026.04 | Verilog HDL, Vivado ILA, Zynq-7015, MCP3004
- **설계** : CdS 센서의 조도를 읽기 위해 10비트 ADC와 통신하는 SPI Mode 0 Master 구현. 50 MHz 시스템 클록 2,500주기마다 SCLK를 토글해 **10 kHz**를 생성하고, 송수신 로직은 같은 시스템 클록에서 에지 스트로브로 제어
- **시작 요청 누락 수정** : 시작 버튼을 눌러도 간헐적으로 CS가 내려가지 않는 현상을 추적. 20 ns짜리 시작 펄스를 SCLK 하강 에지에서만 확인하던 것이 원인이어서, CS가 활성화될 때까지 요청을 플래그에 저장하도록 수정
- **수신 및 보드 검증** : 데이터시트와 ILA 파형을 대조해 **17 SCLK 주기**의 프레임에서 상승 에지 카운터 값이 8, 9일 때 MISO 상위 2비트를 차례로 저장. 센서에 들어오는 빛을 바꿔가며 수신값 00~11이 LED의 **4단계 조도 표시**와 일치하는지 확인

### MEMS 가속도계 설계 및 시뮬레이션

- **기간 / 환경** : 2024년 캡스톤디자인 | MATLAB
- **모델링** : 가속도에 따라 이동 전극이 변위하면 양쪽 전극 간격이 서로 반대 방향으로 변하는 차동 구조를 모델링. 간격 변화가 정전기 강성과 BAW 공진 주파수에 미치는 영향을 계산
- **조건 비교** : 초기 전극 간격을 **100 nm**로 설정하고 바이어스 전압별 주파수 응답을 비교. 전극 간격이 50 nm를 초과하는 조건에서 가속도에 대한 응답의 선형성을 평가
- **담당 및 결과** : 팀원이 같은 조건에서 계산을 재현할 수 있도록 MATLAB 코드 템플릿과 계산 순서도를 작성. 최종 발표에서 **13 V 조건의 선형성 오차를 284.8 ppm**으로 보고

## 📜 자격증

- **OPIc IH (Intermediate High)** | 2026.05
- **데이터분석 준전문가 (ADsP)** | 한국데이터산업진흥원 | 2025.09
- **컴퓨터활용능력 2급** | 대한상공회의소 | 2022.02
- **자동차운전면허 2종 보통** | 2020.04

## 📫 Contact

- **GitHub** : [Riverstone12](https://github.com/Riverstone12)
- **Phone** : 010-3780-4815
- **E-mail** : rivermin3@gmail.com
