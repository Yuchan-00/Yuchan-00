<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:f97316&height=200&section=header&text=Yuchan&fontSize=64&fontColor=7c2d12&animation=fadeIn&fontAlignY=38&desc=AI%20%C3%97%20Hardware%20Engineer&descAlignY=60&descSize=20&descColor=7c2d12" width="100%" alt="Yuchan banner" />

<a href="https://github.com/Yuchan-00/EAD_Engineer_Skill"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=F97316&center=true&vCenter=true&width=720&lines=Building+an+AI+that+designs+electronic+circuits;Deterministic+tools+decide+what+is+true;Verification-first+%C2%B7+KiCad+%C2%B7+SPICE" alt="Typing SVG" /></a>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![SPICE](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=for-the-badge)
![Pydantic](https://img.shields.io/badge/Pydantic_v2-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

**AI × Hardware Engineer**<br>
Building an AI system that designs electronic circuits — with deterministic tools, not LLM guesses, deciding what is true.

</div>

---

## Featured project: [EDA Engineer Skill](https://github.com/Yuchan-00/EAD_Engineer_Skill)

<div align="center">

[![Status](https://img.shields.io/badge/status-in_progress-f97316?style=flat-square)](https://github.com/Yuchan-00/EAD_Engineer_Skill)
[![License](https://img.shields.io/badge/license-proprietary_view--only-f97316?style=flat-square)](https://github.com/Yuchan-00/EAD_Engineer_Skill)
[![Last commit](https://img.shields.io/github/last-commit/Yuchan-00/EAD_Engineer_Skill?style=flat-square&color=f97316)](https://github.com/Yuchan-00/EAD_Engineer_Skill/commits)

</div>

An **agent skill** (in progress): a verification-first electronics design engineer, built from the [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer) reference system. It targets any agent that loads Agent Skills (SKILL.md) or an MCP skill connector.

| In the repository | What it holds |
|---|---|
| [`notes/PLAN.md`](https://github.com/Yuchan-00/EAD_Engineer_Skill/blob/HEAD/notes/PLAN.md) | Setup status, understanding of AI_EDA_Engineer, improvement points, extension plan, next steps |
| [`notes/meetings/`](https://github.com/Yuchan-00/EAD_Engineer_Skill/tree/HEAD/notes/meetings) | Design meetings between Claude and Codex |
| [`notes/measurements/`](https://github.com/Yuchan-00/EAD_Engineer_Skill/tree/HEAD/notes/measurements) | Evidence behind every "measured" claim in the plan |

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

## Current work

- **EDA Engineer Skill** — writing the plan first, then `SKILL.md` and `references/`.
- **AI_EDA_Engineer** — adding circuit templates, most recently a **UHF FM walkie-talkie for perfboard** (amateur 430–440 MHz, discrete parts).

## Tech

| Area | Stack |
|---|---|
| **Languages** | Python |
| **Hardware / EDA** | KiCad, ngspice (SPICE), ERC/DRC, PCB & perfboard design |
| **AI** | LLM orchestration with deterministic validation |

## Connect

- Email: [yuchan.fbu@gmail.com](mailto:yuchan.fbu@gmail.com)
- Issues and PRs are welcome on [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer).

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:f97316,100:ffffff&height=100&section=footer" width="100%" alt="footer" />
