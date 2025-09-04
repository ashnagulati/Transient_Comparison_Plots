# Transient Radio Luminosity (8-10 GHz) and Energy–Velocity Plots

This repository contains curated datasets and plotting scripts used to explore the radio luminosity, temporal evolution, and energy–velocity phase space of astrophysical transients. The sources include gamma-ray bursts (GRBs), tidal disruption events (TDEs), supernovae (SNe), fast blue optical transients (FBOTs), changing-look AGN (CL-AGN), and other rare classes, alongside our new source ASKAP J0055–2558.

## Contents
- [Energy–Velocity plots](./Energy_Velocity_Plot/) — notebook to build E–v phase-space figures and CSVs.
- [Luminosity–Time plots](./Luminosity_Time_Plot/) — notebook for radio luminosity vs. time and CSVs.

## Methodology
- Radio luminosities are calculated from flux densities and distances, with k-corrections applied where appropriate.
- Transients are grouped into physical classes (e.g., GRBs, jetted TDEs, thermal TDEs, SNe, FBOTs).
- ASKAP J0055–2558 is highlighted as a new candidate for comparison across parameter space.

## Requirements
- `pandas`, `numpy`, `matplotlib`, `scipy`, `astropy`, `jupyter`

## Quickstart

### 1) Clone and install requirements
```bash
git clone https://github.com/ashnagulati/Transient_Comparison_Plots.git
cd Transient_Comparison_Plots
pip install pandas numpy matplotlib scipy astropy jupyter
```

### 2) Reproduce figures
`jupyter notebook  # then open the notebooks under Energy_Velocity_Plot/ and Luminosity_Time_Plot/`

---

##  Citation & Attribution

If you use data from this repository, please cite both the original sources (as listed in the accompanying .bib and .RTF files) **and** Gulati et al. (2025, ApJ).



