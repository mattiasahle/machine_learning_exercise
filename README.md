# Machine Learning: Activity Recognition with Neural Networks

> **💡 Tip:** Press `Ctrl+Shift+V` in VS Code to open this README in preview mode.

## Setup

### 1. Create Virtual Environment

```bash
python3 -m venv venv
```

### 2. Activate Virtual Environment

**Linux/macOS:**
```bash
source venv/bin/activate
```

**Windows:**
```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Open Notebook in VS Code

1. Open `ml_activity_recognition_journey.ipynb`
2. Click the kernel selector (top-right corner)
3. Select "Python Environments..." → Choose `venv`
4. Run cells sequentially (Shift+Enter)

## Dataset Structure

```
data/cleaned/acc_mag_gyro/
├── train/          # Training data
├── test/           # Test data
└── test/all/       # Sequential test recordings
```

**File types:**
- `*_acc*.csv` - Accelerometer (ax, ay, az)
- `*_gyro*.csv` - Gyroscope (gx, gy, gz)

## Requirements

- Python 3.8+
- CPU only (no GPU required)
- ~2-3 hours to complete

## Technical Specifications

- **Model:** LSTM neural network (~200K parameters)
- **Input:** 256 timesteps × 6 features
- **Output:** 4 activity classes (run, walk, jump, pushup)
- **Accuracy:** ~95% on test set
