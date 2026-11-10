# Campus3D EnvSim Suite v0.1.7 BETA — Release Notes

**Snapshot date:** 2026-11-10  
**Platform:** Windows / Blender 4.5 LTS  
**Type:** Pre-release / education and research beta

## What changed since v0.1.5 BETA

- Student-first Workflow, four-stage guided UI and automatic grouping of engine N-tabs.
- Calendar date picker and weather preview; single Student flow from selecting/previewing weather to ALL Start.
- Student default: **24-hour previous-day warm-up using actual prior-day weather**, with thermal state carried into selected day; Researcher spin-up modes (real start date, periodic cycles, original 24h CSV).
- Continuous overall progress display across warm-up and target-day runs.
- Info-only warnings do not unnecessarily interrupt Student; real blockers still stop the calculation.
- Temperature legend avoids exaggerated color differences for very narrow ranges, and shows actual data span.
- Viewport legend shows saved JST date/time and outdoor air temperature Ta at matching index, if available; warns when Ta is outside scale.
- Previous/Next stops cleanly at first/last available result index.
- Post-Sim hides overlapping original terrain/building geometry for thermal previews; MP4 output path clarified.
- Patch Limit default 500,000 and capacity/preflight guidance improvements.

## Components

| Extension | Version |
|---|---|
| EnvSim | 0.9.19 |
| GroundPrep | 0.3.2 |
| TreePrep | 0.3.0 |
| MeteoPrep | 0.2.0 |
| ModelPrep | 0.3.3 |
| Pre-Sim | 0.2.2 |
| Simulation | 0.1.2 |
| Post-Sim | 0.3.9 |
| Workflow | 0.4.9 |

## Validation and caveats

Selected operations on Blender 4.5.14 LTS have been confirmed with Shibuya/Kashiwazaki scenes **using the individually updated module builds**. The newly assembled all-in-one installer has passed only offline checks, **not fresh-machine Blender runtime QA**. Keep this release marked **Pre-release**.

The model is intentionally simplified. Student's one-day warm-up is a practical default, not a convergence guarantee. Absolute temperature agreement, parameter uncertainty, GIS model height fidelity and scenario robustness need further evaluation. **Campus3D Tools and QGIS/GSI2Campus3D are not bundled or modified.** GIS Feedback and Ensemble Analysis are future work, not included functionality.

## Install

Download `Campus3D_EnvSim_Suite_v0.1.7_BETA.zip`, unzip it, run `Check_EnvSim_Suite.cmd`, then `Install_EnvSim_Suite.cmd` and type `INSTALL`. Do not pass the Suite ZIP to Blender Install from Disk; the nine extension ZIPs are inside `packages/`.

See `README_FIRST_JA.md` inside the Suite archive.
