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
- [x] 템플릿: 분압기, LED, RC 저역통과, BJT 비안정, ATmega128 개발 보드, 한국 447 MHz 무전기 보드 5종
- [x] 라이선스: MIT + Commons Clause (2026-11-11)
- [ ] 템플릿 더 넣기: LC 저역통과, BJT 로우사이드 스위치, I²C 풀업
- [ ] 계산값 대신 실제로 파는 부품 값 (IEC 60063 E 계열)
- [ ] 템플릿 없는 회로를 설계 파일로 작성
- [ ] 남은 KiCad 검사(실크 DRC, 3D 내보내기)를 KiCad가 있는 기계에서 실행

### [CanSat EDF Rocket](https://github.com/Yuchan-00/CanSat_EDF_Rocket)

![Status](https://img.shields.io/badge/status-v0.9_design_%26_simulation-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/CanSat_EDF_Rocket?style=flat-square&label=last%20commit&color=555555)

<p align="center">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_rocket.jpg" height="260" alt="로켓 구성 (CAD 렌더)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_vtol.jpg" height="260" alt="VTOL 시험 기체 (CAD 렌더)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/pcb_carrier.jpg" height="260" alt="아비오닉스 캐리어 PCB rev 3.1 (KiCad 렌더)">
  <br>
  <sub>로켓 · VTOL 시험 기체 · 아비오닉스 캐리어 PCB rev 3.1 - CAD와 KiCad 렌더이고 사진이 아닙니다</sub>
</p>

90 mm 전기 덕티드팬(EDF) 하나로 나는 3D 프린트 발사체입니다. 캔위성을 싣고 올라가 모터를 끄고, 정점에서 캔위성을 내보낸 뒤 자체 낙하산으로 내려옵니다. 같은 추진 모듈로 가벼운 VTOL 시험 기체도 만들었습니다.

**Ø120 mm PLA 몸통 · 6S 90 mm EDF · 배기 베인 4개 · ATmega128A × 4 비행 컴퓨터 · 4층 캐리어 PCB**

- [x] 로켓과 VTOL의 v0.9 CAD, CadQuery와 Fusion 360으로 교차 확인
- [x] 6자유도 비행 시뮬레이션과 자세 제어
- [x] 칩 4개의 펌웨어, simavr 공동 시뮬레이션
- [x] 캐리어 PCB rev 3.1: 칩 4개 · ESP-12F · 센서를 한 장에, 5 V 승압 회로 내장, ERC/DRC 0, 배선 규칙 21/21 (도구 검사만, 아직 만들지 않음)
- [ ] 로켓에도 캐리어 PCB 넣기 (작업 중, 브랜치 `rocket-carrier`)
- [ ] 첫 실물 조립에서 맞지 않은 베인 서보 연결부 다시 설계 (작업 중)
- [ ] 로켓 기준 펌웨어·시뮬레이션 라운드 (베인 유격 보상 포함)
- [ ] EDF 추력 측정
- [ ] 첫 2색 시험 출력
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
- [x] Templates: divider, LED, RC low-pass, BJT astable, ATmega128 dev board, five KR 447 MHz radio boards
- [x] License: MIT with the Commons Clause (2026-11-11)
- [ ] More templates: LC low-pass, BJT low-side switch, I²C pull-ups
- [ ] Part values that are actually sold (IEC 60063 E series) instead of solved numbers
- [ ] Circuits without a template, written as a design file
- [ ] Run the remaining KiCad checks (silkscreen DRC, 3D export) on a KiCad machine

### [CanSat EDF Rocket](https://github.com/Yuchan-00/CanSat_EDF_Rocket)

A 3D-printed launch vehicle on a single 90 mm electric ducted fan. It carries a CanSat up, cuts the motor, releases the CanSat at apogee and comes down on its own parachute. The same propulsion module also makes a lighter VTOL test vehicle.

**Ø120 mm PLA body · 90 mm EDF on 6S · 4 exhaust vanes · 4 × ATmega128A flight computer · 4-layer carrier PCB**

- [x] v0.9 CAD for the rocket and the VTOL, cross-checked between CadQuery and Fusion 360
- [x] 6-DOF flight simulation and attitude control
- [x] Firmware for all four chips, co-simulated in simavr
- [x] Carrier PCB rev 3.1: 4 chips, ESP-12F and sensors on one board, on-board 5 V boost, ERC/DRC clean, routing rules 21/21 (tool checks only, not manufactured yet)
- [ ] Carrier PCB in the rocket too (in progress, branch `rocket-carrier`)
- [ ] Redesign the vane servo coupling that did not fit in the first real assembly (in progress)
- [ ] Rocket firmware and simulation round (including vane backlash compensation)
- [ ] Measure EDF thrust
- [ ] First two-color test print
- [ ] PCB fabrication and bring-up on real chips
- [ ] Ground radio range test, then first flight

---

**연락 · Contact** · [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
