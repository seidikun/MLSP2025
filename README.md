# Manifold Alignment for Transfer Learning in EEG-based BCI

This repository contains all code and analysis notebooks for the paper:

> **Evaluating Manifold Alignment of Motor Imagery for Transfer Learning in EEG-Based BCIs**  
> Yonamine Yamauti et al., MLSP 2025

---

## Repository Structure

```
.
├── data/                        # (Empty) Place the raw EEG dataset here
├── preprocessed_data/           # Contains preprocessed EEG data for direct use in analysis
├── results/                     # Stores processed results (e.g., accuracy tables, plots)
├── notebooks/                   # All Jupyter/Colab notebooks for each analysis step
│   ├── preprocessing.ipynb
│   ├── [Data Extraction] inter_session_riemannian_alignment.ipynb
│   ├── [Analysis] inter_session_riemannian_alignment.ipynb
│   ├── [Data Extraction] inter_subject_riemannian_alignment.ipynb
│   ├── [Analysis] inter_subject_riemannian_alignment.ipynb
│   └── [Analysis] inter_subject_riemannian_alignment_high_acc.ipynb
├── requirements.txt
└── README.md
```

---

## Notebooks Overview

- **preprocessing.ipynb**  
  Preprocesses raw EEG data. You need to download the dataset (see below) and set the folder paths in the notebook to match your Google Drive or local structure.

- **[Data Extraction] inter_session_riemannian_alignment.ipynb**  
  Performs within-subject (inter-session) Riemannian alignment and feature extraction.

- **[Analysis] inter_session_riemannian_alignment.ipynb**  
  Loads processed inter-session data and generates statistical analysis and plots.

- **[Data Extraction] inter_subject_riemannian_alignment.ipynb**  
  Performs inter-subject Riemannian alignment and feature extraction.

- **[Analysis] inter_subject_riemannian_alignment.ipynb**  
  Loads processed inter-subject data and generates statistical analysis and plots.

- **[Analysis] inter_subject_riemannian_alignment_high_acc.ipynb**  
  Analysis and visualization focused on the subset of high-performing subjects.

---

## Data Access & Preprocessing

1. **Download the raw EEG dataset**  
   This project uses the [Jeong et al., 2020 multimodal EEG dataset](https://doi.org/10.1038/s41597-020-00695-5), also available at [GigaDB](http://gigadb.org/dataset/view/id/100788).  
   - Download the data and place it in the `data/` folder.

2. **Preprocessing**  
   - Open `notebooks/preprocessing.ipynb` in Google Colab (or locally).
   - **Important:** Update the file paths to match the location of your data in Google Drive or your local system.
   - This script will generate preprocessed datasets saved in `preprocessed_data/` for further analysis.

---

## Results

- All processed results (accuracy tables, plots, etc.) will be saved in the `results/` folder.
- Figures in the paper can be reproduced by running the respective [Analysis] notebooks.

---

## Dependencies

- Python 3.8+
- numpy, scipy, scikit-learn, matplotlib, pandas, mne, and Jupyter/Colab

Install dependencies with:
```bash
pip install -r requirements.txt
```

---

## Reproducing the Analysis

1. Preprocess the data using `preprocessing.ipynb`.
2. Run the [Data Extraction] notebooks for feature extraction and alignment.
3. Use the [Analysis] notebooks to generate all figures and statistical summaries.

---

## Citation

If you use this code, please cite:

```bibtex
@inproceedings{yamauti2025mlsp,
  title={Evaluating Manifold Alignment of Motor Imagery for Transfer Learning in EEG-Based BCIs},
  author={Yonamine Yamauti, S. and others},
  booktitle={IEEE International Workshop on Machine Learning for Signal Processing (MLSP)},
  year={2025}
}
```

---

## Contact

For questions or contributions, please open an issue or contact [seidi.yamaut@gmail.com](mailto:seidi.yamaut@gmail.com).

---

*This repository accompanies the MLSP 2025 submission.*
