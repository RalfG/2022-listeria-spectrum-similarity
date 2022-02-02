# 2022-listeria-spectrum-similarity

![GitHub release](https://img.shields.io/github/v/release/ralfg/2022-listeria-spectrum-similarity)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5948475.svg)](https://doi.org/10.5281/zenodo.5948475)

Code and results for similarity calculation between endogenous and synthetic Listeria peptide
spectra.

---

### Replicating the results

#### Binder online notebook

Open this repo in Binder:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/RalfG/2022-listeria-spectrum-similarity/HEAD?labpath=2022-listeria-spectrum-similarity.ipynb)

#### Local setup

Requirements: Miniconda or Anaconda installation

- Clone this repository: `git clone https://github.com/RalfG/2022-listeria-spectrum-similarity`
- Open the directory: `cd 2022-listeria-spectrum-similarity`
- Create the conda environment: `conda env create -f environment.yml`
- Activate the environment: `conda activate spectrum_similarity`
- Start a local Jupyter server: `jupyter notebook`
- Open the notebook file `2022-listeria-spectrum-similarity.ipynb` and run all cells.

### Files
Input:
- `input/peptides.csv`: CSV with peptides in [ProForma2 notation](https://www.psidev.info/proforma)
- `input/spectra/*.csv`: One CSV file per spectrum with the columns `MS2 m/z` and `Relative Intensity in %`

Output:
- `output/correlations.csv`: Pearson correlation per pair of spectra
- `output/mirror_plots.zip`: Visualizations of mirrored spectra with annotated peaks
