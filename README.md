# IRCM-breastcancer

This repository contains the data processing, modeling, and analysis code used to construct the Breast Cancer Multivariate Risk Index (IRCM) and to study breast cancer mortality patterns using integrated socioeconomic, healthcare, and environmental data.

## Overview

Breast cancer mortality is influenced by multiple structural factors that are often studied in isolation. This project proposes an interpretable multivariate framework that integrates heterogeneous data sources into a single composite risk index.

The IRCM captures territorial risk by combining:
- Socioeconomic marginalization
- Healthcare infrastructure
- Environmental exposure to carcinogenic emissions

The framework is designed to support:
- Analysis of spatial disparities in mortality
- Identification of high-risk municipalities
- Interpretable modeling of structural risk
- Short-term forecasting of risk dynamics

## Data Sources

All data used in this project are publicly available:

- **Mortality data**: INEGI (2000–2022), breast cancer deaths by municipality and age group  
- **Population data**: INEGI demographic data for rate calculation  
- **Environmental data**: SEMARNAT pollutant emissions (IARC Group 1 and 2 carcinogens)  
- **Healthcare infrastructure**: CLUE registry (medical units and mammography devices)  
- **Socioeconomic indicators**: CONAPO marginalization index (2020)

## Methodology

The workflow consists of the following steps:

1. Data integration and harmonization across sources  
2. Min–max normalization of all variables  
3. Correlation analysis using Spearman’s rank coefficient  
4. Construction of the IRCM as a weighted linear combination of variables  
5. Exploratory analysis of latent structure using PCA  
6. Linear modeling to assess association with mortality  
7. Time-series forecasting using autoregressive Random Forest models  

## Key Features

- Interpretable composite risk index (IRCM)
- Integration of heterogeneous public datasets
- Spatially explicit analysis at the municipal level
- Combination of statistical and machine learning approaches
- Reproducible pipeline in Python

## Repository Structure
