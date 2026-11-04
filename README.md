<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:f97316&height=200&section=header&text=Yuchan&fontSize=64&fontColor=7c2d12&animation=fadeIn&fontAlignY=38&desc=AI%20%C3%97%20Hardware%20Engineer&descAlignY=60&descSize=20&descColor=7c2d12" width="100%" alt="Yuchan banner" />

<a href="https://github.com/Yuchan-00/EDA_Engineer_Skill"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=F97316&center=true&vCenter=true&width=720&lines=Building+an+AI+that+designs+electronic+circuits;Deterministic+tools+decide+what+is+true;Verification-first+%C2%B7+KiCad+%C2%B7+SPICE" alt="Typing SVG" /></a>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![SPICE](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=for-the-badge)
![Pydantic](https://img.shields.io/badge/Pydantic_v2-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

**AI × Hardware Engineer**<br>
Building an AI system that designs electronic circuits — with deterministic tools, not LLM guesses, deciding what is true.

</div>

---

## Featured project: [EDA Engineer Skill](https://github.com/Yuchan-00/EDA_Engineer_Skill)

<div align="center">

[![Status](https://img.shields.io/badge/status-in_progress-f97316?style=flat-square)](https://github.com/Yuchan-00/EDA_Engineer_Skill)
[![License](https://img.shields.io/badge/license-proprietary_view--only-f97316?style=flat-square)](https://github.com/Yuchan-00/EDA_Engineer_Skill)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/EDA_Engineer_Skill?style=flat-square&color=f97316)](https://github.com/Yuchan-00/EDA_Engineer_Skill/commits)

</div>

An **agent skill** (in progress): a verification-first electronics design engineer, built from the [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer) reference system. It targets any agent that loads Agent Skills (SKILL.md) or an MCP skill connector.

| In the repository | What it holds |
|---|---|
| [`notes/PLAN.md`](https://github.com/Yuchan-00/EDA_Engineer_Skill/blob/HEAD/notes/PLAN.md) | Setup status, understanding of AI_EDA_Engineer, improvement points, extension plan, next steps |
| [`notes/meetings/`](https://github.com/Yuchan-00/EDA_Engineer_Skill/tree/HEAD/notes/meetings) | Design meetings between Claude and Codex |
| [`notes/measurements/`](https://github.com/Yuchan-00/EDA_Engineer_Skill/tree/HEAD/notes/measurements) | Evidence behind every "measured" claim in the plan |

The skill itself (`SKILL.md` + `references/`) is not written yet; the plan comes first. The repository is public to read, under a proprietary view-only license.

---

## Reference system: [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

<div align="center">

[![Stars](https://img.shields.io/github/stars/Yuchan-00/AI_EDA_Engineer?style=flat-square&logo=github&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer)
[![Forks](https://img.shields.io/github/forks/Yuchan-00/AI_EDA_Engineer?style=flat-square&logo=github&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/forks)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/AI_EDA_Engineer?style=flat-square&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/commits)
[![Issues](https://img.shields.io/github/issues/Yuchan-00/AI_EDA_Engineer?style=flat-square&color=f97316)](https://github.com/Yuchan-00/AI_EDA_Engineer/issues)

</div>

The system the skill is built from: a **verification-first** AI engineering system for electronic circuit design. It takes a natural-language requirement through one pipeline:

`requirements` → `parts & regulatory research` → `Universal Circuit IR` → `calculations / SPICE` → `KiCad schematic & PCB` → `ERC / DRC` → `manufacturing outputs` → `independent review` → `auto-fix`

> **Core principle:** the LLM never decides design truth. It only proposes and orchestrates — facts come from the IR, provenance, deterministic tools (calculators, SPICE, KiCad ERC/DRC, manufacturing-file checks) and an independent reviewer.

### Highlights

| Feature | What it does |
|---|---|
| **Universal Circuit IR** | Pydantic v2 model with content-based design hashes |
| **Provenance for every value** | user requirement / authoritative / assumption / derived / LLM-generated |
| **Conservative validation** | PASS / FAIL / NOT_VERIFIED / USER_INPUT_REQUIRED, never optimistic |
| **Real SPICE + KiCad** | ngspice simulation and KiCad 10 ERC/DRC in the loop |

### Quick start

After installing (see the [repository](https://github.com/Yuchan-00/AI_EDA_Engineer) for details):

```bash
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
| **Airframe** | Ø120 mm body printed on a Bambu Lab P2S in PLA Matte, YUCHAN logo inlaid in two colours |
| **Propulsion & control** | 90 mm 12-blade EDF on 6S; attitude held by 4 exhaust vanes driven directly by MG90S servos |
| **Flight computer** | 4 × ATmega128A (NAV · FCU · COM · GNS) at 250 Hz; LoRa link to a laptop ground station |
| **Payload** | Standard CanSat, Ø66 × 115 mm, 350 g |

It follows the same rule as my EDA work: **design values come from one source (`params.json`), and tools decide pass or fail.**

- CadQuery geometry checks (C1–C36), cross-checked against an independent Fusion 360 model
- Real Bambu Studio slicing for mass, print time and colour changes
- 6-DOF flight simulation with campaigns, plus a 4-chip firmware co-simulation in simavr
- Every number labelled as measured, estimated or assumed, with an independent review each round

> **Not flown yet.** EDF thrust has not been measured and nothing has been printed or flight-tested; current numbers come from CAD, the slicer and simulation.

---

## Current work

- **EDA Engineer Skill** — writing the plan first, then `SKILL.md` and `references/`.
- **AI_EDA_Engineer** — adding circuit templates, most recently a **UHF FM walkie-talkie for perfboard** (amateur 430–440 MHz, discrete parts).
- **CanSat EDF Rocket** — v0.9: lighter VTOL configuration, direct-drive vanes, a motor-lead passage that fits without measuring, and the white body with the YUCHAN logo. Next: porting the v0.9 control changes to firmware, then thrust testing.

## Tech

| Area | Stack |
|---|---|
| **Languages** | Python |
| **Hardware / EDA** | KiCad, ngspice (SPICE), ERC/DRC, PCB & perfboard design |
| **Embedded** | ATmega128A, C (avr-gcc, PlatformIO), simavr co-simulation, LoRa |
| **Mechanical / CAD** | CadQuery, Fusion 360 API, Bambu Studio, 3D printing |
| **Simulation** | 6-DOF flight simulation in Python |
| **AI** | LLM orchestration with deterministic validation |

## Connect

- Email: [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
- Issues and PRs are welcome on [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer).

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f97316,100:ffffff&height=100&section=footer" width="100%" alt="footer" />
