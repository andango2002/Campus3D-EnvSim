# Campus3D Sim Suite v0.1.10 BETA — Thermal GLB Shared Comparison Scale

This pre-release updates the existing 10-extension Campus3D Sim Suite for **Blender 4.5 LTS**.

## Highlights

- **Post-Sim upgraded from v0.3.9 to v0.3.12**.
- Thermal GLB includes **GROUND, ROOF, WALL surface temperatures** alongside **SET*, MRT or estimated WBGT**.
- Human metric and Surface Temperature are now encoded using **one shared temperature color range**, allowing direct visual comparison of temperatures in the same 3D scene.
- Distinct, labeled legends remain embedded in the GLB to identify the quantities.
- Other nine extension archives are preserved **byte-for-byte** from v0.1.9 BETA. Teaching-only Campus3D Tools and QGIS plugins are not included or modified.

## Included extensions

Sim Tools 0.1.0 | Workflow 0.4.14 | Pre-Sim 0.2.3 | EnvSim 0.9.20 | GroundPrep 0.3.3 | Simulation 0.1.2 | **Post-Sim 0.3.12** | ModelPrep 0.3.3 | TreePrep 0.3.0 | MeteoPrep 0.2.0

## Installation — Windows, Blender 4.5 LTS

1. Close Blender, extract `Campus3D_Sim_Suite_v0.1.10_BETA_Release.zip`.
2. Run `Check_Campus3D_Sim_Suite.cmd` and confirm `10 / 10 PASS`.
3. Run `Install_Campus3D_Sim_Suite.cmd`, review changes, and enter `INSTALL`.
4. Restart Blender. Export SET* + Surface T from Post-Sim v0.3.12.

## Validation / limitations

The user confirmed GLB display with matching color limits and ground/building surface temperatures in an external glTF viewer. Package structure, checksums, embedded extension manifest versions and Python syntax were checked offline. This **integrated installer has not yet been tested on a clean Windows/Blender installation**. Thermophysiological/scientific validity is not certified.
