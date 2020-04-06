# mce-data-ccsa

This repository contains climate model data processed from output of the Coupled Model Intercomparison Project phase 5 (CMIP5) and phase 6 (CMIP6). The data files are in netCDF format and to be linked in `mce/data/preproc[12]` of [Minimal CMIP Emulator (MCE)](https://github.com/tsutsui1872/mce).

`preproc1` contains globally-averaged, yearly-aggregated data for the top-of-atmosphere energy imbalance (`rtnt`) and the surface air temperature (`tas`); `preproc2` contains their anomaly data. File names are in the following format:
```
preproc1/<variable>_<model>_<experiment>.nc
preproc2/<variable>_<model>_<experiment>_anom.nc
```
where `<variable>` is `rtnt` or `tas`, `<model>` is one of the dataset names described in [`references.md`](./references.md), and `<experiment>` is one of the CMIP experiments, such as `abrupt-4xCO2`, `1ptcCO2`, and `piControl`. These are the atmospheric CO<sub>2</sub> increase experiments for abrupt quadrupling and transient 1%-per-year increase, and the preindustrial control.

See Jupyter notebooks in the MCE repository for details.
