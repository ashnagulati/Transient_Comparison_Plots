# Transient Radio Luminosity (8-10 GHz) and Energy–Velocity Plots

This repository contains curated datasets and plotting scripts used to explore the radio luminosity, temporal evolution, and energy–velocity phase space of astrophysical transients. The sources include gamma-ray bursts (GRBs), tidal disruption events (TDEs), supernovae (SNe), fast blue optical transients (FBOTs), changing-look AGN (CL-AGN), and other rare classes, alongside our new source ASKAP J0055–2558.

## Contents
- **Data**: CSV files containing 8-10 GHz luminosity values, time, energy, and velocity measurements. Each file corresponds to a transient class or a specific object.
- **Plots**: Python scripts to generate:
  - Luminosity vs. time plots
  - Energy vs. velocity plots

## Methodology
- Radio luminosities are calculated from flux densities and distances, with k-corrections applied where appropriate.
- Transients are grouped into physical classes (e.g., GRBs, jetted TDEs, thermal TDEs, SNe, FBOTs).
- ASKAP J0055–2558 is highlighted as a new candidate for comparison across parameter space.

## Requirements
- `pandas`, `numpy`, `matplotlib`, `scipy`

## Usage
1. Clone this repo:
   ```bash
   git clone https://github.com/ashnagulati/Transient_Comparison_Plots.git

---

##  Citation & Attribution

If you use data from this repository, please cite both the original sources (as listed in the accompanying .bib and .RTF files) **and** Gulati et al. (2025, ApJ).



