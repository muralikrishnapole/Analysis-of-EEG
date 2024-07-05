# Analysis-of-EEG
This project focuses on analyzing EEG data to classify cognitive states using deep learning. The dataset is from the [Mental Arithmetic Tasks Dataset](https://physionet.org/content/eegmat/1.0.0/) at PhysioNet, pre-cleaned for immediate use. For more insights, refer to the accompanying [research paper](https://www.mdpi.com/2306-5729/4/1/14).
# Repository: EEG Cognitive State Classification

## Overview
This repository contains the code and documentation for analyzing and classifying cognitive states using EEG data and advanced deep learning techniques. The dataset used is the **Mental Arithmetic Tasks Dataset**, sourced from PhysioNet ([dataset link](https://physionet.org/content/eegmat/1.0.0/)). This dataset includes pre-cleaned EEG recordings taken during mental arithmetic tasks and rest states, enabling focused efforts on model implementation and evaluation.

The accompanying research paper provides further insights into the dataset and its applications, which can be reviewed [here](https://www.mdpi.com/2306-5729/4/1/14).

## Objectives
The goal of this assignment is to:
1. Analyze the EEG data and perform Power Spectral Density (PSD) analysis.
2. Implement and evaluate multiple deep learning models to classify cognitive states.

Specifically, you will:
- Load and preprocess the EEG data.
- Perform PSD analysis to identify differences in frequency bands between rest and task states.
- Implement at least two deep learning models from the suggested list to classify cognitive states.
- Evaluate the performance of these models using standard metrics.


## Steps to Achieve It

### 1. Load the EEG Data
- **Dataset Preparation**: Download the EEG data from PhysioNet. Ensure the data is structured and accessible for analysis.
- **Data Loading**: Use the MNE library to load the EEG data into the workspace for processing.

### 2. Power Spectral Density (PSD) Analysis
- **Frequency Bands**: Analyze the EEG data in the following frequency bands: 
  - Delta (1-4 Hz)
  - Theta (4-8 Hz)
  - Alpha (8-12 Hz)
  - Beta (12-30 Hz)
  - Gamma (30-100 Hz)
- **State Comparison**: Calculate and compare the band-wise PSD for both rest (recording EEG dataset before the mental arithmetic task) and task states (recording EEG dataset during the mental arithmetic task).
- **Summary of Findings**: Document the differences in PSD between the two states and interpret the implications.

### 3. Deep Learning Classification
- **Feature Extraction**: Extract relevant features from the EEG data that can be used for classification.
- **Model Implementation**: Implement at least two different deep learning models from the following:
  - EEGNet
  - TSCeption
  - ViT (Vision Transformer)
  - ATCNet
  - VAE (Variational Autoencoder)
- **Model Training and Validation**: Train and validate the models using the EEG dataset. Split the data appropriately for training and testing.
- **Model Evaluation**: Evaluate the performance of the models using metrics such as accuracy, precision, recall, and F1-score. Discuss the results and compare the performance of the models.

## How to Use This Repository
1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/yourusername/eeg-cognitive-state-classification.git
   ```
2. **Install Dependencies**: 
   Ensure you have Python 3.8 or higher. Install required packages using:
   ```bash
   pip install -r requirements.txt
   ```
3. **Download and Prepare Data**:
   Follow the instructions in the `data/` directory to download and organize the EEG dataset from PhysioNet.

4. **Run Jupyter Notebooks**:
   Open and execute the notebooks in the `notebooks/` directory to reproduce the analysis and model results.

## Dependencies
- Python 3.8+
- Jupyter Notebook
- MNE
- TensorFlow or PyTorch (depending on model implementation)
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## Results and Discussion
The `results/` directory contains the outputs of the models, including:
- Trained model weights
- Evaluation metrics
- Visualizations of PSD and model performance

Detailed discussion of the results and interpretations are provided in the Jupyter Notebooks.

## Contributions
Feel free to fork this repository, make improvements, and submit pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## References
- [PhysioNet EEGMAT Dataset](https://physionet.org/content/eegmat/1.0.0/)
- [Research Paper on Dataset](https://www.mdpi.com/2306-5729/4/1/14)
