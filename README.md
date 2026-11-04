<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:f97316&height=200&section=header&text=Yuchan&fontSize=64&fontColor=7c2d12&animation=fadeIn&fontAlignY=38&desc=AI%20%C3%97%20Hardware%20Engineer&descAlignY=60&descSize=20&descColor=7c2d12" width="100%" alt="Yuchan banner" />

<a href="https://github.com/Yuchan-00/EDA_Engineer_Skill"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=F97316&center=true&vCenter=true&width=720&lines=Building+an+AI+that+designs+electronic+circuits;Deterministic+tools+decide+what+is+true;Verification-first+%C2%B7+KiCad+%C2%B7+SPICE;Also%3A+a+3D-printed+EDF+rocket+for+CanSats" alt="Typing SVG" /></a>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![SPICE](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=for-the-badge)
![CadQuery](https://img.shields.io/badge/CadQuery-2B3137?style=for-the-badge)
![Fusion 360](https://img.shields.io/badge/Fusion_360-F97316?style=for-the-badge)

**AI × Hardware Engineer**<br>
Building an AI system that designs electronic circuits, and a 3D-printed EDF rocket for CanSats.<br>
In both, deterministic tools decide what is true, not LLM guesses.

</div>

---

## About

I work across circuit design (KiCad, SPICE), embedded firmware (AVR) and 3D-printed flight hardware, and I build each one the same way: every value has a source, every number says whether it was measured, estimated or assumed, and a tool or an independent reviewer decides pass or fail.

---

## Featured project: [EDA Engineer Skill](https://github.com/Yuchan-00/EDA_Engineer_Skill)

<div align="center">

[![Status](https://img.shields.io/badge/status-planning-f97316?style=flat-square)](https://github.com/Yuchan-00/EDA_Engineer_Skill)
[![License](https://img.shields.io/badge/license-proprietary_view--only-f97316?style=flat-square)](https://github.com/Yuchan-00/EDA_Engineer_Skill)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/EDA_Engineer_Skill?style=flat-square&color=f97316)](https://github.com/Yuchan-00/EDA_Engineer_Skill/commits)

</div>

An **agent skill** that turns any agent loading Agent Skills (SKILL.md) or an MCP skill connector into a verification-first electronics design engineer, built from [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer). The repository currently holds the plan ([`notes/PLAN.md`](https://github.com/Yuchan-00/EDA_Engineer_Skill/blob/HEAD/notes/PLAN.md)), the design meetings between Claude and Codex ([`notes/meetings/`](https://github.com/Yuchan-00/EDA_Engineer_Skill/tree/HEAD/notes/meetings)) and the evidence behind every measured claim ([`notes/measurements/`](https://github.com/Yuchan-00/EDA_Engineer_Skill/tree/HEAD/notes/measurements)). Public to read, under a proprietary view-only license.

---

## Reference system: [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

<div align="center">

[![Stars](https://img.shields.io/github/stars/Yuchan-00/AI_EDA_Engineer?style=flat-square&logo=github&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer)
[![Forks](https://img.shields.io/github/forks/Yuchan-00/AI_EDA_Engineer?style=flat-square&logo=github&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/forks)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/AI_EDA_Engineer?style=flat-square&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/commits)
[![Issues](https://img.shields.io/github/issues/Yuchan-00/AI_EDA_Engineer?style=flat-square&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/issues)

</div>

A **verification-first** AI engineering system for electronic circuit design. It takes a natural-language requirement through one pipeline:

`requirements` → `parts & regulatory research` → `Universal Circuit IR` → `calculations / SPICE` → `KiCad schematic & PCB` → `ERC / DRC` → `manufacturing outputs` → `independent review` → `auto-fix`

> **Core principle:** the LLM never decides design truth. It only proposes and orchestrates — facts come from the IR, provenance, deterministic tools (calculators, SPICE, KiCad ERC/DRC, manufacturing-file checks) and an independent reviewer.

| Feature | What it does |
|---|---|
| **Universal Circuit IR** | Pydantic v2 model with content-based design hashes |
| **Provenance for every value** | user requirement / authoritative / assumption / derived / LLM-generated |
| **Conservative validation** | PASS / FAIL / NOT_VERIFIED / USER_INPUT_REQUIRED, never optimistic |
| **Real SPICE + KiCad** | ngspice simulation and KiCad 10 ERC/DRC in the loop |

**Quick start** — one line installs the code, Python, KiCad 10 and ngspice (macOS / Linux; Windows and options in the [repository](https://github.com/Yuchan-00/AI_EDA_Engineer)):

```bash
curl -fsSL https://raw.githubusercontent.com/Yuchan-00/AI_EDA_Engineer/main/install.sh | bash
ai-eda doctor      # check your environment
ai-eda gui --open  # launch the local web GUI
```

---

## Also building: [CanSat EDF Rocket](https://github.com/Yuchan-00/CanSat_EDF_Rocket)

<div align="center">

[![Status](https://img.shields.io/badge/status-v0.9_design_%26_simulation-f97316?style=flat-square)](https://github.com/Yuchan-00/CanSat_EDF_Rocket)
[![MCU](https://img.shields.io/badge/MCU-ATmega128A_%C3%974-f97316?style=flat-square)](https://github.com/Yuchan-00/CanSat_EDF_Rocket/tree/HEAD/firmware)
[![License](https://img.shields.io/badge/license-CC_BY--NC_4.0-f97316?style=flat-square)](https://github.com/Yuchan-00/CanSat_EDF_Rocket/blob/HEAD/LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/CanSat_EDF_Rocket?style=flat-square&color=f97316)](https://github.com/Yuchan-00/CanSat_EDF_Rocket/commits)

<a href="https://github.com/Yuchan-00/CanSat_EDF_Rocket"><img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_rocket.jpg" width="300" alt="CanSat EDF Rocket, rocket configuration (CAD render)" /></a>
<a href="https://github.com/Yuchan-00/CanSat_EDF_Rocket"><img src="https://raw.githubusercontent.com/Yuchan-00/CanSat_EDF_Rocket/main/docs/images/hero_vtol.jpg" width="300" alt="CanSat EDF Rocket, VTOL battery configuration (CAD render)" /></a>
<br>
<sub>Rocket configuration (left) and VTOL battery configuration (right). CAD renders, not photos.</sub>

</div>

A **3D-printed launch vehicle powered by a single 90 mm electric ducted fan (EDF)** that carries a CanSat up, cuts the motor, opens the nose cone at apogee to release the CanSat, and comes down on its own parachute. The same propulsion module also forms a lighter **VTOL test vehicle** in battery, tethered and hybrid power configurations.

| Part | What it is |
|---|---|
| **Airframe** | Ø120 mm body printed on a Bambu Lab P2S in PLA Matte, YUCHAN logo inlaid in two colors |
| **Propulsion & control** | 90 mm 12-blade EDF on 6S; attitude held by 4 exhaust vanes driven directly by MG90S servos |
| **Flight computer** | 4 × ATmega128A (NAV · FCU · COM · GNS) at 250 Hz; LoRa link to a laptop ground station |
| **Payload** | Standard CanSat, Ø66 × 115 mm, 350 g |

Design values come from one source (`params.json`) and are checked by CadQuery geometry checks (C1–C36) cross-checked against an independent Fusion 360 model, real Bambu Studio slicing, a 6-DOF flight simulation, and a 4-chip firmware co-simulation in simavr.

> **Not flown yet.** EDF thrust has not been measured and nothing has been printed or flight-tested; current numbers come from CAD, the slicer and simulation.

---

## Current work

- **EDA Engineer Skill** — writing the plan first, then `SKILL.md` and `references/`.
- **AI_EDA_Engineer** — adding circuit templates, most recently a **UHF FM walkie-talkie for perfboard** (amateur 430–440 MHz, discrete parts).
- **CanSat EDF Rocket** — v0.9 brought a lighter VTOL configuration, direct-drive vanes, a motor-lead passage that fits without measuring, and the white body with the YUCHAN logo. Next: porting the v0.9 control changes to firmware, then thrust testing.

## Tech

| Area | Stack |
|---|---|
| **Languages** | Python, C |
| **Hardware / EDA** | KiCad, ngspice (SPICE), ERC/DRC, PCB & perfboard design |
| **Embedded** | ATmega128A, avr-gcc, PlatformIO, simavr co-simulation, LoRa |
| **Mechanical / CAD** | CadQuery, Fusion 360 API, Bambu Studio, 3D printing |
| **Simulation** | 6-DOF flight simulation in Python |
| **AI** | LLM orchestration with deterministic validation |

## Connect

- Email: [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
- Issues and PRs are welcome on [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer); questions and feedback on [CanSat EDF Rocket](https://github.com/Yuchan-00/CanSat_EDF_Rocket/issues).

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f97316,100:ffffff&height=100&section=footer" width="100%" alt="footer" />
