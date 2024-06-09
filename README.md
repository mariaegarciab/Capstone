# Bearing Data Analysis and Feature Engineering

## Introduction

This project focuses on the analysis and feature engineering of vibration data from bearings. The objective is to develop predictive maintenance models that can identify bearing failures before they occur. The data is sourced from the IMS Bearing Dataset, which consists of multiple test-to-failure experiments.

## Dataset Description

- **Bearing Configuration**: Four bearings were installed on a shaft with a constant rotation speed of 2000 RPM, powered by an AC motor. A radial load of 6000 lbs was applied to the shaft and bearings using a spring mechanism.
- **Sensors**: PCB 353B33 High Sensitivity Quartz ICP accelerometers were installed on the bearing housing to collect vibration data.
- **Data Structure**: Each dataset contains 1-second vibration signal snapshots recorded at specific intervals. Each file contains 20,480 data points sampled at 20 kHz.
- **Test-to-Failure**: Data was collected until bearing failure, which occurred after exceeding the designed lifetime of over 100 million revolutions.

## Project Structure

- **1st_test**: Directory containing data from the first test-to-failure experiment.
- **2nd_test**: Directory containing data from the second test-to-failure experiment.
- **3rd_test**: Directory containing data from the third test-to-failure experiment.
- **capstone_indra.ipynb**: Jupyter Notebook with the data analysis, feature engineering, and visualization code.
- **dataset1_features.csv**: Extracted features from the first dataset.
- **dataset2_features.csv**: Extracted features from the second dataset.
- **dataset3_features.csv**: Extracted features from the third dataset.
- **desc_stats1.csv**: Descriptive statistics for the first dataset.
- **desc_stats2.csv**: Descriptive statistics for the second dataset.
- **desc_stats3.csv**: Descriptive statistics for the third dataset.

## Feature Engineering

The feature engineering process involves extracting meaningful features from the vibration data to help in predictive modeling. The features include:

- **Time-Domain Features**:
  - Root Mean Square (RMS)
  - Mean Absolute Value (MAV)
  - Kurtosis
  - Entropy

- **Frequency-Domain Features**:
  - Fast Fourier Transform (FFT)
  - Spectral Entropy

## Visualizations

Several visualizations were created to gain insights into the data and the extracted features:

- **Time-Domain Features**: Line plots of RMS, Kurtosis, and Entropy over time.
- **Descriptive Statistics**: Summary statistics for each feature.
- **Distribution Plots**: Histograms and box plots to visualize the distribution of each feature.
- **Pair Plots**: Pairwise relationships between features to identify potential correlations.

## How to Run the Project

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/mariaegarciab/Capstone.git
   cd Capstone
