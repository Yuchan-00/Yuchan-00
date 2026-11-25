<div align="center">

# Yuchan

**AI × Hardware Engineer**

전자 회로를 설계하는 AI와, 캔위성을 싣는 3D 프린트 EDF 로켓을 만듭니다.<br>
모든 숫자에는 출처가 있고, 합격·불합격은 도구가 정합니다.

<sub>Building an AI that designs electronic circuits, and a 3D-printed EDF rocket for CanSats. Every number has a source; tools decide pass or fail.</sub>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![ngspice](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=flat-square)
![ATmega128A](https://img.shields.io/badge/ATmega128A-AVR-555555?style=flat-square)
![CadQuery](https://img.shields.io/badge/CadQuery-2B3137?style=flat-square)
![Fusion 360](https://img.shields.io/badge/Fusion_360-F97316?style=flat-square)

**한국어** · [English](#english)

</div>

---

### [EDA Engineer Skill](https://github.com/Yuchan-00/EDA_Engineer_Skill)

![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/EDA_Engineer_Skill?style=flat-square&label=last%20commit&color=555555)

Claude Code, Codex처럼 Agent Skills를 읽는 에이전트를 검증 우선 전자회로 설계 엔지니어로 만드는 에이전트 스킬(`SKILL.md` + 참고 문서)입니다. 아래 AI_EDA_Engineer의 `ai-eda` CLI를 움직입니다.

- [x] Claude Code와 Codex용 `SKILL.md`, 참고 문서, 결과 전달 스크립트
- [x] 결과 전달: 요약·상세 PDF 보고서(한국어 또는 영어)와 KiCad 프로젝트·거버·BOM·CPL을 묶은 zip 하나
- [x] 두 스킬 폴더가 같은지 보는 이식성 검사와 시험
- [x] 라이선스: MIT + Commons Clause

### [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

![Status](https://img.shields.io/badge/status-active-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/AI_EDA_Engineer?style=flat-square&label=last%20commit&color=555555)

검증 우선의 AI 회로 설계 시스템입니다. LLM은 제안만 하고, 무엇이 맞는지는 회로 IR, SPICE, KiCad ERC/DRC와 독립 검토가 정합니다.

`요구사항` → `LLM 에이전트가 제안` → `회로 IR (값 + 출처)` → `SPICE · KiCad ERC/DRC` → `독립 검토` → `거버 · BOM`

- [x] 요구사항에서 거버·BOM까지 이어지는 전체 파이프라인, 로컬 웹 GUI
- [x] macOS, Linux, Windows 한 줄 설치 (Python, KiCad 10, ngspice)
- [x] 템플릿: 분압기, LED, RC 저역통과, LC 저역통과, BJT 비안정, BJT 로우사이드 스위치, I²C 풀업, ATmega128 개발 보드, 한국 447 MHz 무전기 보드 5종
- [x] 계산값 대신 실제로 파는 부품 값 (IEC 60063 E 계열)
- [x] 템플릿 없는 회로를 설계 파일로 작성 (`ai-eda run --design`)
- [x] 다층 배선(2 → 12층), 둥근 모서리 배선, SI·크로스토크 검사
- [x] 모든 회로도를 교과서식으로 그림 (전원선 위, 신호 왼쪽 → 오른쪽, 되먹임 위)
- [x] 주문용 출력: 확인 안 된 칸은 비워 두고 이유를 적는 BOM, 거버 좌표계의 부품 중심 CPL, 측정용 테스트 포인트
- [x] 라이선스: MIT + Commons Clause (2026-11-11)
- [ ] 첫 실물 시험 PCB: 9 V 8음 아날로그 화음 피아노 (TL082 / LM324, 서랍 부품, 테스트 포인트 14개) 주문 준비
- [ ] 남은 KiCad 검사(실크 DRC, 3D 내보내기)를 KiCad가 있는 기계에서 실행

### [CanSat EDF Rocket with ATmega128](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128)

📐 [블록도 · 순서도](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128#블록도--순서도) - 시스템, 전원, 항공전자, 기체 구성, 비행·사출 순서, 펌웨어 상태, 제어 루프, 개발 흐름

![Status](https://img.shields.io/badge/status-v1.0_new_body_design-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128?style=flat-square&label=last%20commit&color=555555)

<p align="center">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/main/cad/body_v2/out/render/body_v2_iso.png" height="260" alt="새 본체 v1.0 (CAD 렌더)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/main/cad/body_v2/out/render/body_v2_cut.png" height="260" alt="새 본체 v1.0 반 단면 (CAD 렌더)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/main/docs/images/pcb_carrier.jpg" height="260" alt="아비오닉스 캐리어 PCB rev 3.1 (KiCad 렌더)">
  <br>
  <sub>새 본체 v1.0 · 단면 · 아비오닉스 캐리어 PCB rev 3.1 (CAD · KiCad 렌더)</sub>
</p>

90 mm 전기 덕티드팬(EDF) 하나로 나는 3D 프린트 발사체입니다. 캔위성을 싣고 올라가 정점에서 캔위성을 내보낸 뒤 낙하산으로 내려옵니다.

**PLA 몸통 · 6S 90 mm EDF · 배기 베인 4개 · ATmega128A × 4 비행 컴퓨터 · 4층 캐리어 PCB**

- [x] 칩 4개의 펌웨어, 6자유도 비행 시뮬레이션, simavr 공동 시뮬레이션
- [x] 캐리어 PCB rev 3.1: 칩 4개 · ESP-12F · 센서를 한 장에, 5 V 승압 회로 내장, ERC/DRC 0, 배선 규칙 21/21
- [x] 실제 로켓 팀이 쓰는 도구로 검증: OpenRocket · RocketPy · OpenFOAM ([보고서](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/blob/main/sim/validation_2026-11-18/README.md))
- [x] **새 본체 v1.0** ([CAD v2](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/tree/main/cad/body_v2)): 질량 2,089 g (CanSat 없이), 정적 안정 여유 +1.09 cal
- [x] PLA 지상시험 EDF 로터: 잰 구동 홈에 맞춰 시험 상한 11,000 rpm ([설계](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/blob/main/docs/EDF_로터_설계.md))
- [ ] EDF 추력 측정
- [ ] 벤치 시험: 진동, 로터 지상 시험
- [ ] 새 본체 자세 제어·펌웨어
- [ ] PCB 제작과 실제 칩 동작 확인
- [ ] 지상 무선 거리 시험, 그다음 첫 비행

---

## English

### [EDA Engineer Skill](https://github.com/Yuchan-00/EDA_Engineer_Skill)

An agent skill (`SKILL.md` + references) that turns Claude Code, Codex or any agent that loads Agent Skills into a verification-first electronics design engineer. It drives the `ai-eda` CLI of AI_EDA_Engineer below.

- [x] `SKILL.md`, references and a hand-over script for Claude Code and Codex
- [x] Hand-over: summary and detailed PDF reports (Korean or English) and one zip with the KiCad project, Gerbers, BOM and CPL
- [x] Portability check that keeps the two skill folders identical, with tests
- [x] License: MIT with the Commons Clause

### [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

A verification-first AI system for circuit design. The LLM only proposes; the circuit IR, SPICE, KiCad ERC/DRC and an independent reviewer decide what is true.

`Requirement` → `LLM agents propose` → `Circuit IR (value + source)` → `SPICE · KiCad ERC/DRC` → `Independent review` → `Gerber · BOM`

- [x] Full pipeline from requirement to Gerber and BOM, with a local web GUI
- [x] One-line installer for macOS, Linux and Windows (Python, KiCad 10, ngspice)
- [x] Templates: divider, LED, RC low-pass, LC low-pass, BJT astable, BJT low-side switch, I²C pull-ups, ATmega128 dev board, five KR 447 MHz radio boards
- [x] Part values that are actually sold (IEC 60063 E series) instead of solved numbers
- [x] Circuits without a template, written as a design file (`ai-eda run --design`)
- [x] Multilayer routing (2 → 12 layers), rounded-corner tracks, SI and crosstalk checks
- [x] Every schematic drawn textbook style (supply on top, signal left to right, feedback above)
- [x] Order-ready outputs: a BOM that leaves unverified cells empty and says why, a CPL with part centres in the Gerbers' frame, test points for measurement
- [x] License: MIT with the Commons Clause (2026-11-11)
- [ ] First real test PCB: a 9 V eight-voice analog chord piano (TL082 / LM324, drawer parts, 14 test points), being prepared for order
- [ ] Run the remaining KiCad checks (silkscreen DRC, 3D export) on a KiCad machine

### [CanSat EDF Rocket with ATmega128](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128)

📐 [Block diagrams and flowcharts](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/blob/main/README.en.md#block-diagrams--flowcharts) (labels in Korean): system, power, avionics, airframe stack, flight and ejection sequence, firmware states, control loop, development flow

![Status](https://img.shields.io/badge/status-v1.0_new_body_design-f97316?style=flat-square)

A 3D-printed launch vehicle on a single 90 mm electric ducted fan. It carries a CanSat up, releases it at apogee and comes down on a parachute.

**PLA body · 90 mm EDF on 6S · 4 exhaust vanes · 4 × ATmega128A flight computer · 4-layer carrier PCB**

- [x] Firmware for all four chips, 6-DOF flight simulation, simavr co-simulation
- [x] Carrier PCB rev 3.1: 4 chips, ESP-12F and sensors on one board, on-board 5 V boost, ERC/DRC clean, routing rules 21/21
- [x] Checked with the tools real rocket teams use: OpenRocket · RocketPy · OpenFOAM ([report, Korean](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/blob/main/sim/validation_2026-11-18/README.md))
- [x] **New body v1.0** ([CAD v2](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/tree/main/cad/body_v2)): mass 2,089 g (without CanSat), static margin +1.09 cal
- [x] PLA ground-test EDF rotor: test cap 11,000 rpm for the measured drive slot ([design, Korean](https://github.com/Yuchan-00/CanSat_EDF_Rocket_with_ATmega128/blob/main/docs/EDF_로터_설계.md))
- [ ] Measure EDF thrust
- [ ] Bench tests: vibration, rotor ground test
- [ ] Attitude control and firmware for the new body
- [ ] PCB fabrication and bring-up on real chips
- [ ] Ground radio range test, then first flight

---

**연락 · Contact** · [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
