# Depression-Detection-Using-Machine-Learning-Approaches
A Hybrid Energy-Attention Transformer (HEAT) for text-based depression detection using Transformer, TF-IDF priors, and energy-based inference.

# Repository Structure
```
Source code
│
├── Data Preprocessing
│   ├── D1_D2_PREPROCESS.ipynb
│   └── DAIC_PREPROCESS.ipynb
│
└── Model
    ├── HEAT_D1.ipynb
    ├── HEAT_D2.ipynb
    └── HEAT_D3.ipynb
```

## Dataset
This project is based on three publicly available datasets.
The Kaggle repository contains:
- The collected and organized datasets used in this project.
- The preprocessed dataset, along with the training, validation, and testing datasets used for the experiments.
Download the complete dataset from Kaggle:
https://kaggle.com/datasets/ee25765f37847f78000ef7aecdb36a795539cf8cd8672c0f6e314edd48254d41
The training, validation, and testing datasets have been preprocessed and split to ensure reproducibility.

# Data Preprocessing
This folder contains the preprocessing notebooks used to prepare the datasets before model training.
- **D1_D2_PREPROCESS.ipynb** – Preprocessing for Dataset 1 and Dataset 2.
- **DAIC_PREPROCESS.ipynb** – Preprocessing for Dataset 3 (DAIC-WOZ).
> **Important**
>
> Before running the preprocessing notebooks, update all dataset file paths according to your local environment or Google Drive location.

# Model

This folder contains the implementation of the proposed **HEAT (Hybrid Energy-Attention Transformer)** model.
Each notebook corresponds to one dataset.
| Notebook | Dataset |
|----------|---------|
| HEAT_D1.ipynb | Dataset 1 |
| HEAT_D2.ipynb | Dataset 2 |
| HEAT_D3.ipynb | Dataset 3 (DAIC-WOZ) |
Run the notebook corresponding to the dataset you wish to reproduce.

# Software Requirements
The project was developed using:
- Python 3.10+
- Jupyter Notebook
- Google Colab
The experimental results reported in this project were generated using **Google Colab with an NVIDIA A100 GPU**.
> **Note:** Running the model on CPU is possible but not recommended due to the significantly longer training time.


# Required Libraries
Install the required libraries before running the notebooks.
```bash
pip install torch
pip install transformers
pip install datasets
pip install accelerate
pip install sentencepiece
pip install scikit-learn
pip install pandas
pip install numpy
pip install matplotlib
pip install nltk
pip install tqdm
pip install emoji
```
Additional libraries may be required depending on the notebook.
