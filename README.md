# Machinery Fault Diagnosis and Prognosis

This repository contains a prototype machine learning model designed to predict real-time machinery failures. It utilizes probabilistic deep learning techniques combined with specifically tailored features extracted from vibration data provided by the NASA IMS Bearing Data.

## Project Overview

This project was developed as a proof of concept for the research: "real-time machinery fault diagnosis and prognosis using probabilistic deep learning integrated with tailored features." The model processes vibration data from bearings to predict potential failures, aiding in preemptive maintenance and operational optimization.

## Dataset

The dataset used is from NASA's Prognostics Data Repository, specifically the `IMS Bearing Data`. This data was generated with support from Rexnord Corp, and contains several datasets where each consists of vibration data recorded from bearings until failure.

Resource: https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/
Download: https://data.nasa.gov/download/brfb-gzcv/application%2Fzip

### Data Description

- **Data Sets**: Three test-to-failure experiment datasets.
- **Sampling Rate**: 20 kHz, with each file representing 1 second of vibration data.
- **Features**: Vibration data from multiple channels depending on the bearing and experiment setup.

## Machine Learning Pipeline

1. **Data Preprocessing**:
   - Merging data from multiple files to create a unified dataset.
   - Cleaning and structuring data for analysis.

2. **Exploratory Data Analysis**:
   - Visualizing vibration data to understand patterns and anomalies.

3. **Feature Engineering**:
   - Extracting meaningful features from raw data to enhance model predictions.

4. **Model Development**:
   - Developing separate models using Sequential and CNN architectures.

5. **Training and Evaluation**:
   - Training models on the processed data and evaluating their performance.

## Usage

To run this project, ensure you have Python and the necessary libraries installed:

```bash
pip install numpy pandas matplotlib tensorflow scikit-learn
