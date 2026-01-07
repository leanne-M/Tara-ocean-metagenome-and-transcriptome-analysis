# Tara ocean metagenome and metatranscriptome figure generation 

This repository contains R scripts used to analyse the abundance, distribution, and expression of genes in global marine metagenomic and metatranscriptomic datasets. 

## Overview
The analyses quantify gene and transcript abundances across depth profiles (surface, deep chlorophyll maximum, and mesopelagic waters), assess relationships with environmental nutrient concentrations, and compare gene and transcript prevalence.

All statistical analyses were performed on normalised gene and transcript abundance data.

## Contents
- `analysis/` – R scripts for statistical analyses, and figure generation  
- `figures/` – Scripts used to generate figures included in the thesis  
- `README.md` – Project description and usage information

## Data sources
Metagenomic and metatranscriptomic data were obtained from the **Tara Oceans** project and are subject to their respective data-use policies. Raw sequencing data are not included in this repository but can be found using this link https://tara-oceans.mio.osupytheas.fr

Environmental metadata (e.g. phosphate concentrations) were sourced from publicly available Tara Oceans datasets https://tara-oceans.mio.osupytheas.fr.

## Methods summary
- Phytase genes (*bpP* and *cypH*) were identified using Hidden Markov Models (HMMs) constructed from curated reference sequences.  
- Gene and transcript abundances were normalised to expected genome counts prior to analysis.  
- Spearman’s rank correlations were used to assess monotonic relationships between normalised abundances and environmental phosphate concentrations.  
- Visualisation was performed using `ggplot2`, `ggpubr`, and `patchwork`.

## Reproducibility
This repository contains all scripts required to reproduce the analyses and figures presented in the associated thesis, provided that the relevant Tara Oceans datasets are obtained independently.

## Code availability
All code is provided for transparency and reproducibility.

## Author
Leanne Murray

