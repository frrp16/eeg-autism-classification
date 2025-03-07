# EEG Autism Classification

## Overview
This repository contains code and resources for classifying Autism Spectrum Disorder (ASD) using EEG signals. The project explores different feature extraction techniques and evaluates their effectiveness in distinguishing ASD subjects from control subjects.

## Dataset
The dataset used in this project is provided by **King Abdul Aziz University** and can be accessed at the following link:
[BCI Datasets - King Abdul Aziz University](https://malhaddad.kau.edu.sa/Pages-BCI-Datasets-En.aspx)

The dataset includes EEG recordings from ASD and control subjects. The metadata files provide details about subjects, recording conditions, and EEG channel information.

## Notebooks
The repository includes Jupyter notebooks for different stages of the classification pipeline:

### 1. Data Visualization
- Exploratory analysis of EEG signals.
- Signal plotting and basic preprocessing.

### 2. Feature Extraction
- **Relative Wavelet Bispectrum (RWB)**
- **Bispectrum**
- **Fast Fourier Transform (FFT)**
- **Discrete Wavelet Transform (DWT)**

### 3. Modeling
- Multilayer Perceptron (MLP) models trained using extracted features.
- Evaluates classification performance of different feature extraction methods.
- Results indicate that **Bispectrum-based methods achieve higher accuracy** compared to FFT and DWT.

## Environment Setup
To set up the environment, install dependencies using the provided `environment.yml` file:
```sh
conda env create -f environment.yml
conda activate eeg-autism-classification
```

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/frrp16/eeg-autism-classification.git
   cd eeg-autism-classification
   ```
2. Activate the conda environment:
   ```sh
   conda activate eeg-autism-classification
   ```
3. Open Jupyter Notebook and run the analysis:
   ```sh
   jupyter notebook
   ```

## References
- [BCI Datasets - King Abdul Aziz University](https://malhaddad.kau.edu.sa/Pages-BCI-Datasets-En.aspx)
- [EEG-Based Computer Aided Diagnosis of Autism Spectrum Disorder Using Wavelet, Entropy, and ANN](https://onlinelibrary.wiley.com/doi/10.1155/20179816591)
- [Development of Filtered Bispectrum for EEG Signal Feature Extraction in Automatic Emotion Recognition Using Artificial Neural Networks](https://www.mdpi.com/1999-4893/10/2/63)
- [Relative wavelet bispectrum feature for alcoholic EEG signal classification using artificial neural network](https://ieeexplore.ieee.org/document/8168473)
