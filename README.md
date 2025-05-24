# Manifold Alignment for Transfer Learning in EEG-based BCI

This repository contains the code and analysis scripts used in the study:

> **Evaluating Manifold Alignment of Motor Imagery for Transfer Learning in EEG-Based BCIs**  
> Yonamine Yamauti et al., MLSP 2025

## Overview

This project investigates whether motor imagery (MI) representations in EEG data can be aligned across sessions and subjects to improve decoding generalization, using Riemannian geometry, dimensionality reduction, and Procrustes-based alignment. All code for preprocessing, feature extraction, statistical analysis, and visualization is provided here.

## Main Features

- Preprocessing of raw EEG data (bandpass filtering, epoching)
- Extraction of covariance features and tangent space projection (Riemannian geometry)
- Dimensionality reduction with PCA
- Alignment using Procrustes analysis and hyperalignment
- Classification with logistic regression
- Statistical evaluation (Wilcoxon signed-rank test)
- Visualization of results (accuracy curves, boxplots, PCA projections)

## Repository Structure

