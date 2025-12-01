# Transient Radio Luminosity (8-10 GHz) and Energy–Velocity Plots

This repository contains curated datasets and plotting scripts used to explore the radio luminosity temporal evolution, and energy–velocity phase space of astrophysical synchrotron transients. The data include radio observations from diverse transient classes (e.g. Gamma‑Ray Bursts (GRBs), Tidal Disruption Events (TDEs), Supernovae (SNe), Fast Blue Optical Transients (FBOTs), changing-look AGN (CL-AGN), and other rare classes), plus a newly identified source: ASKAP J0055–2558. This repo supports the analysis and figures presented in the associated paper (Gulati et al. 2025, ApJ), as well as enabling reuse of the curated data and plotting workflows by other researchers.

## Repository Contents

### 1) Data Files 

All data files are provided in CSV format within the data directories, organized by transient class. These files contain:
- Source name / identifier
- Redshift or host-galaxy distance in `Mpc`
- Time post explosion in `days`
- Observed flux densities with uncertainties in `mJy`
- Observation frequency in `GHz`
- Classification (GRB, TDE, SN, FBOT, CL-AGN, etc.)
- Observed kinetic energies in `erg` and velocities as $`\Gammma\beta`$

### 2) Jupyter Notebooks

The data directories include Jupyter notebooks — for data processing, plotting, and generating figures:
- [Energy–Velocity plots](./Energy_Velocity_Plot/) — notebook to build E–v phase-space figures and CSVs.
- [Luminosity–Time plots](./Luminosity_Time_Plot/) — notebook for radio luminosity vs. time and CSVs.

### 3) References

The directories also contain bibliographic files such as:
- `.bib` files — citations for all observational data sources
- `.rtf` or `.txt` reference lists — original sources of radio measurements used in the paper

## Methodology
- **Band:** All CSV radio data are **8–10 GHz** only
- **Luminosity:** $`L_\nu = 4\pi D_L^2\,S_\nu\,(1+z)`$ 
- **GRBs:** Bulk $`\Gamma \approx 1/\theta_j`$ unless a direct $`\Gamma`$ is reported
- **Classes:** short-/long-GRBs, jetted/thermal/delayed TDEs, Type II/rebrightening SNe, FBOTs, AGN
- **Candidate:** Highlight **ASKAP J0055–2558** for comparison


## Requirements
- `pandas`, `numpy`, `matplotlib`, `scipy`, `astropy`, `jupyter`

## Quickstart

### 1) Clone and install requirements
```bash
git clone https://github.com/ashnagulati/Transient_Comparison_Plots.git
cd Transient_Comparison_Plots
pip install pandas numpy matplotlib scipy astropy jupyter
jupyter notebook
```

### 2) Reproduce figures
Then open the notebooks under [Energy–Velocity plots](./Energy_Velocity_Plot/) and [Luminosity–Time plots](./Luminosity_Time_Plot/) 

The notebooks take raw observational radio data (flux densities, redshifts, times) and compute physical quantities: e.g., luminosities (with k-correction), co-moving distances, transformations needed for cosmology, etc. Light-curves and phase-space (energy vs. velocity) plots are generated for various transient classes — allowing comparison across classes (GRBs, TDEs, SNe, FBOTs, CL-AGN, ASKAP J0055–2558, etc.). CSV files have been provided for ease of reuse — enabling external analysis without re-running the full notebooks. The workflow reproduces the figures and comparative analyses presented in the associated publication (Gulati et al. 2025, ApJ).
Thus, the code and data are tightly integrated with the science paper: the repo enables reproduction, verification, and further reuse of the analyses.

---

##  Citation & Attribution

If you use data from this repository, please cite both the original sources (as listed in the accompanying `.bib` and `.RTF` files) **and** the main paper: **Gulati et al. (2025, ApJ)**.



