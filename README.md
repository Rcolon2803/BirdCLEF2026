# BirdCLEF 2026 Bioacoustic Classification Project

This repository contains my BirdCLEF 2026 machine learning project focused on bioacoustic species classification using audio recordings from the Kaggle BirdCLEF+ 2026 competition.

The goal of this project is to identify animal species from sound recordings by combining exploratory audio analysis, feature engineering, baseline modeling, and a Kaggle-ready submission pipeline.

## Project Overview

This project was developed locally in **VS Code** and later adapted into a **Kaggle notebook submission pipeline** for competition use.

The workflow includes:
- metadata exploration
- waveform and spectrogram analysis
- segmented audio feature extraction
- baseline classification modeling
- Kaggle submission notebook development

## Development Environment

Local development was completed in **VS Code**, where the project was organized, tested, and debugged before being prepared for Kaggle execution.

The final submission workflow was adapted for **Kaggle Notebooks**, where the competition notebook environment is required for private test-set scoring.

## Important Note About Data

Raw competition data is **excluded from this repository**.

This includes:
- training audio
- test soundscapes
- raw metadata files provided by Kaggle

Because BirdCLEF 2026 is a Kaggle competition with hidden test data, the full submission process must be executed inside Kaggle’s competition notebook environment.

## Notebooks

### `01_eda.ipynb`
Exploratory data analysis notebook covering:
- metadata inspection
- class distribution
- recording quality
- geographic distribution
- waveform and spectrogram visualization
- comparison of insect and bird acoustic patterns

### `02_baseline_model.ipynb`
Baseline modeling notebook covering:
- segmented 5-second audio windows
- MFCC and delta-based feature extraction
- Random Forest baseline classification
- validation experiments on a lightweight subset of frequent classes

### `03_kaggle_inference.ipynb`
Kaggle submission notebook covering:
- competition path setup
- training subset reconstruction
- segmented feature extraction
- baseline model training
- grouped soundscape inference
- `submission.csv` generation for Kaggle

## Methods Used

This project currently uses:
- Python
- pandas
- NumPy
- librosa
- scikit-learn
- Jupyter notebooks
- VS Code
- Kaggle Notebooks

## Project Structure

```text
BirdCLEF/
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_baseline_model.ipynb
│   └── 03_kaggle_inference.ipynb
├── src/
├── models/
├── outputs/
├── README.md
└── requirements.txt
