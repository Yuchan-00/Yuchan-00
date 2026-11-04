<div align="center">

# Hi, I'm Yuchan 👋

**AI × Hardware Engineer**<br>
Building an AI system that designs electronic circuits — with deterministic tools, not LLM guesses, deciding what is true.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![SPICE](https://img.shields.io/badge/ngspice-SPICE-4B8BBE?style=for-the-badge)
![Pydantic](https://img.shields.io/badge/Pydantic_v2-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

</div>

---

## 🚀 Featured project: [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer)

A **verification-first** AI engineering system for electronic circuit design. It takes a natural-language requirement through one pipeline:

`requirements` → `parts & regulatory research` → `Universal Circuit IR` → `calculations / SPICE` → `KiCad schematic & PCB` → `ERC / DRC` → `manufacturing outputs` → `independent review` → `auto-fix`

**Core principle:** the LLM never decides design truth. It only proposes and orchestrates — facts come from the IR, provenance, deterministic tools (calculators, SPICE, KiCad ERC/DRC, manufacturing-file checks) and an independent reviewer.

### Highlights

🧩 **Universal Circuit IR** — Pydantic v2 model with content-based design hashes<br>
🧾 **Provenance for every value** — user requirement / authoritative / assumption / derived / LLM-generated<br>
✅ **Conservative validation** — PASS / FAIL / NOT_VERIFIED / USER_INPUT_REQUIRED, never optimistic<br>
📐 **Deterministic calculators** — Ohm's law, dividers, RC, thermal, RF and more, each traceable<br>
🔬 **Real SPICE + KiCad** — ngspice simulation and KiCad 10 ERC/DRC in the loop<br>
🖥️ **One-line install & local web GUI** — `ai-eda doctor`, `ai-eda gui --open`

## 📡 Latest work

Adding circuit templates — most recently a **UHF FM walkie-talkie for perfboard** (amateur 430–440 MHz, discrete parts).

## 🧰 In progress

**EAD Engineer Skill** — an Agent Skill (SKILL.md) that packages the AI_EDA_Engineer workflow for agents that load skills. *Private repository, in development.*<br>
Status (2026-11-04): planning phase · 6 of 17 roadmap steps done.

## 🛠️ Tech

**Languages** · Python<br>
**Hardware / EDA** · KiCad, ngspice (SPICE), ERC/DRC, PCB & perfboard design<br>
**AI** · LLM orchestration with deterministic validation

## 📫 Connect

Issues and PRs are welcome on [AI_EDA_Engineer](https://github.com/Yuchan-00/AI_EDA_Engineer).
