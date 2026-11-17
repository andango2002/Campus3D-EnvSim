# Campus3D Sim Suite v0.1.9 BETA — Independent Sim Tools + Student MRT Auto Recovery

This release is a separate research/education thermal analysis suite for Blender 4.5 LTS, consisting of **10 extensions**, including the independent `campus3d_sim_tools` imported from the successful Phase 1/2 implementation.

## Changes since v0.1.8

- **Independent Campus3D Sim Tools v0.1.0** (QGIS manifest import and physical-Z correction); original `campus3d_tools` is not included, installed, or altered. Keep stable **Campus3D Tools v0.4.18** as the Latest release of its own project.
- **Workflow v0.4.13**: Phase 2 bridge retained; Student (GUIDED) auto-applies a verified Pre-Sim MRT grid recommendation **only when it is the sole BLOCK**, once per ALL Start; immediate live revalidation; failures and risk warnings are not bypassed; changes are recorded inside the Blender scene.
- **Pre-Sim v0.2.3**: only processes tagged `Campus3D_Sim` models, not legacy teaching model collections.
- Includes tested GroundPrep v0.3.3, EnvSim v0.9.20, Simulation v0.1.2 and the six other pinned modules from v0.1.8.
- Retains physical-Z normalization, GIS GroundPrep Bake, 24h real-weather spin-up, Post-Sim JST/Ta viewport legend, Recovery Flow and capacity checks.

## Quality & limitations

Structural consistency, package hashing and Python syntax are checked offline. User confirmed Phase 2 through completed Simulation and Post-Sim on Blender 4.5.14 LTS. **The newly added Student MRT auto-path and the combined installer have not been tested in a live Blender/Windows installation.** Validation of temperature or MRT against field measurements is a separate research task.

## Installation

Download `Campus3D_Sim_Suite_v0.1.9_BETA_10Extensions.zip`, extract all, run `Check_Campus3D_Sim_Suite.cmd`, then `Install_Campus3D_Sim_Suite.cmd`.

Recommended release tag: `v0.1.9-beta` (**Pre-release**). Campus3D Tools stable Latest stays untouched.
