# Campus3D EnvSim Suite

**Latest pre-release: v0.1.7 BETA (2026-11-10)**  
Educational urban thermal environment simulation suite for Blender 4.5 LTS.

QGIS/3D GIS environment data + historical weather + simplified urban thermal models → surface temperature, MRT, SET* and WBGT; guided Student/Researcher workflows and Post-Sim visualization.

## Download

**[Download Campus3D EnvSim Suite v0.1.7 BETA](https://github.com/andango2002/Campus3D-EnvSim/releases/download/v0.1.7-beta/Campus3D_EnvSim_Suite_v0.1.7_BETA.zip)**

Download the asset from **Releases**, extract the Suite ZIP, then run `Check_EnvSim_Suite.cmd` and `Install_EnvSim_Suite.cmd`. Do **not** pass the top-level Suite ZIP to Blender's Install from Disk. Individual engine ZIPs are in `packages/`.

See [Japanese quick start](docs/STUDENT_QUICKSTART_v0.1.7_JA.md) and [release notes](RELEASE_NOTES_v0.1.7.md).

## Current component versions

Workflow **0.4.9**, EnvSim **0.9.19**, Simulation **0.1.2**; GroundPrep 0.3.2, TreePrep 0.3.0, MeteoPrep 0.2.0, ModelPrep 0.3.3, Pre-Sim 0.2.2, Post-Sim 0.3.9.

## Scope / limitations

- **BETA / Pre-release.** Existing user environment (individual updates) completed spin-up + Student ALL Start + Post-Sim, but freshly assembled Suite's clean-install/update installer has not been GUI tested on a new machine.
- Student mode defaults to a previous-day, 24-hour actual-weather warm-up. Physical fidelity/absolute temperatures are **not validated** for arbitrary streets, models, or weather.
- **Campus3D Tools (3DTools), GSI2Campus3D and QGIS are excluded, not modified, and remain separate projects.**
- GIS Feedback (georeferenced results), A/B scenario and robustness/GIS analyses are next-stage planned capabilities, not present in this release.
- Consult weather data providers' terms; external retrieval depends on network access.

## License

Bundled components declare `SPDX:GPL-3.0-or-later` in their Blender manifests. A copy of GPLv3 is included in the distribution. Third-party assets and any other applicable notices must retain their own conditions.
