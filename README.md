# Machine Learning: Activity Recognition with Neural Networks

> **💡 Tip:** Press `Ctrl+Shift+V` in VS Code to open this README in preview mode.

## Prerequisites

Before starting, ensure you have:
- **Python 3.8+** installed ([python.org](https://www.python.org/downloads/))
- **VS Code** with Python extension ([code.visualstudio.com](https://code.visualstudio.com/))
- **Git** (optional, for cloning the repository)
- Basic Python knowledge (functions, loops, basic syntax)
- Curiosity and 2-3 hours of focused time

**No prior ML experience needed!** The notebook guides you through everything.

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

## Need Help?

**Got stuck? Ran into issues?** Don't hesitate to reach out! Ask questions to:
- **GitHub Copilot, ChatGPT, Claude** or similar AI assistants - they're great at debugging and explaining concepts
- Your peers and colleagues - learning together is more fun!
- The course instructors if this is part of a structured program

Remember: Asking questions is part of learning! 🙋

## Background & Attribution

### Dataset
The sensor data was recorded specifically for this exercise and is provided free of charge for educational purposes.

### Origins
Curious about how this notebook came to be? Check out:
- **`original_lab_report.pdf`** - The original exercise this journey evolved from
- **`DEVELOPMENT_JOURNEY.md`** - A fascinating chronicle of how we transformed a basic lab into this comprehensive learning experience through iterative collaboration (highly recommended read!)

### Pitch
See **`THE_PITCH.md`** for the promotional version of this exercise.
