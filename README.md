# Machine Learning Exercise - Activity Recognition with LSTM

This repository contains a machine learning exercise for classifying human activities using sensor data from accelerometer and gyroscope readings.

## Overview

The notebook `lab4.ipynb` implements an LSTM-based Recurrent Neural Network to classify four different activities:
- Running
- Walking
- Jumping
- Push-ups

## Dataset

The dataset is located in `data/cleaned/acc_mag_gyro/` and contains:
- **Training data** (`train/`): Sensor readings for training the model
- **Test data** (`test/`): Sensor readings for evaluating the model
- **Combined test data** (`test/all/`): Sequential recordings of all activities

Each CSV file contains sensor readings:
- `*_acc*.csv`: Accelerometer data (ax, ay, az)
- `*_gyro*.csv`: Gyroscope data (gx, gy, gz)
- `*_mag*.csv`: Magnetometer data (mx, my, mz)

## Getting Started

### Prerequisites

#### Setting Up a Virtual Environment

It's recommended to use a virtual environment to manage dependencies:

1. **Create a virtual environment:**
```bash
python3 -m venv venv
```

2. **Activate the virtual environment:**
   - On Linux/macOS:
   ```bash
   source venv/bin/activate
   ```
   - On Windows:
   ```bash
   venv\Scripts\activate
   ```

3. **Install the required packages:**
```bash
pip install -r requirements.txt
```

#### Configuring the Notebook in VS Code

1. **Open the notebook** `lab4.ipynb` in VS Code

2. **Select the Python kernel:**
   - Click on the kernel selector in the top-right corner of the notebook (or click "Select Kernel" if no kernel is selected)
   - Choose "Python Environments..."
   - Select the virtual environment you just created (it should appear as `venv` or `./venv/bin/python`)

3. **Verify the kernel:**
   - The top-right corner should now show your selected Python environment
   - If the kernel fails to start, click "Select Kernel" again and refresh the list

### Running the Notebook

Run all cells sequentially to:
- Load and preprocess the data
- Train the LSTM model
- Evaluate performance
- Visualize predictions

## Model Architecture

The model uses:
- Input layer with time series data (256 timesteps)
- LSTM layer with 256 units
- Dropout layer (0.1) for regularization
- Dense output layer with softmax activation (4 classes)

## Key Features

- Cross-platform compatibility (works on Windows, Linux, macOS)
- CPU-only execution (no GPU required)
- Modern pandas/TensorFlow/Keras API usage
- Clean code with no deprecation warnings

## Exercise Goals

This exercise helps you understand:
- Time series classification with deep learning
- LSTM neural networks
- Sensor data processing
- Model evaluation and visualization

## Notes

- The notebook is configured to use CPU only to avoid CUDA issues
- Random seeds are set for reproducible results
- All deprecation warnings have been resolved for modern library versions
