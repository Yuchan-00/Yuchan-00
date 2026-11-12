<div align="center">

# Yuchan

**AI × Hardware Engineer**

Building an AI that designs electronic circuits, and a 3D-printed EDF rocket for CanSats.<br>
Every number has a source; tools decide pass or fail.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![ngspice](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=flat-square)
![ATmega128A](https://img.shields.io/badge/ATmega128A-AVR-555555?style=flat-square)
![CadQuery](https://img.shields.io/badge/CadQuery-2B3137?style=flat-square)
![Fusion 360](https://img.shields.io/badge/Fusion_360-F97316?style=flat-square)

</div>

---

### [EDA Engineer Skill](https://github.com/Yuchan-00/EDA_Engineer_Skill)

![Status](https://img.shields.io/badge/status-first_draft-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/EDA_Engineer_Skill?style=flat-square&label=last%20commit&color=555555)

An agent skill (`SKILL.md` + references) that turns Claude Code, Codex or any agent that loads Agent Skills into a verification-first electronics design engineer. It is built from AI_EDA_Engineer below, and the design meetings between Claude and Codex and the evidence behind every measured claim live in the repo.

- [x] First draft of `SKILL.md` and its references, for Claude Code and Codex
- [x] Tried on real design tasks; trigger tests passed on Claude Code and Codex
- [x] Hand-over step: summary and detailed PDF reports (Korean or English) and one zip of the KiCad project
- [ ] Stronger checks: operating point vs. part ratings (in progress)
- [ ] Readable, wired schematics; simulation with part tolerances and trace parasitics
- [ ] Op-amp and rectifier templates

### [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

![Status](https://img.shields.io/badge/status-active-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/AI_EDA_Engineer?style=flat-square&label=last%20commit&color=555555)

A verification-first AI system for circuit design. The LLM only proposes; the circuit IR, SPICE, KiCad ERC/DRC and an independent reviewer decide what is true.

`Requirement` → `LLM agents propose` → `Circuit IR (value + source)` → `SPICE · KiCad ERC/DRC` → `Independent review` → `Gerber · BOM`

- [x] Full pipeline from requirement to Gerber and BOM, with a local web GUI
- [x] One-line installer for macOS, Linux and Windows (Python, KiCad 10, ngspice)
- [x] Templates: divider, LED, RC low-pass, BJT astable, ATmega128 dev board, five KR 447 MHz radio boards
- [ ] More templates: LC low-pass, BJT low-side switch, I²C pull-ups (built on a work branch)
- [ ] Part values that are actually sold (IEC 60063 E series) instead of solved numbers (six templates done on a work branch)
- [ ] Circuits without a template, written as a design file; test board: STM32F407 display driver (in progress)
- [ ] Run the remaining KiCad checks (silkscreen DRC, 3D export) on a KiCad machine

### [CanSat EDF Rocket](https://github.com/Yuchan-00/CanSat_EDF_Rocket)

![Status](https://img.shields.io/badge/status-v0.9_design_%26_simulation-f97316?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/CanSat_EDF_Rocket?style=flat-square&label=last%20commit&color=555555)

<p align="center">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_rocket.jpg" height="260" alt="Rocket configuration (CAD render)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_vtol.jpg" height="260" alt="VTOL test vehicle (CAD render)">
  <img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/pcb_carrier.jpg" height="260" alt="Avionics carrier PCB (KiCad render)">
  <br>
  <sub>Rocket · VTOL test vehicle · avionics carrier PCB — CAD and KiCad renders, not photos</sub>
</p>

A 3D-printed launch vehicle on a single 90 mm electric ducted fan. It carries a CanSat up, cuts the motor, releases the CanSat at apogee and comes down on its own parachute. The same propulsion module also makes a lighter VTOL test vehicle.

**Ø120 mm PLA body · 90 mm EDF on 6S · 4 exhaust vanes · 4 × ATmega128A flight computer**

- [x] v0.9 CAD for the rocket and the VTOL, cross-checked between CadQuery and Fusion 360
- [x] 6-DOF flight simulation and attitude control
- [x] Firmware for all four chips, co-simulated in simavr
- [x] 4-layer avionics carrier PCB, ERC/DRC clean (not manufactured yet)
- [ ] Measure EDF thrust
- [ ] First two-color test print
- [ ] PCB fabrication and bring-up on real chips
- [ ] Ground radio range test, then first flight

---

**Contact** · [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
