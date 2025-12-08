# CECS 456 Deep Learning Project

**Authors:** Melody Gatan & Matthew Nguyen  
**Course:** CECS 456 - Deep Learning  
**Date:** December 5, 2025

Comparison of VGG16 and ResNet50 architectures on Animals10 dataset.

## How to Run

### Step 1: Open Notebook in Colab

1. Open `VGG16_Animals10.ipynb` or `RestNet.ipynb` in Google Colab
2. Change runtime to GPU: `Runtime` → `Change runtime type` → Select `T4 GPU` or `A100 GPU`

### Step 2: Download Dataset (using Kaggle API)

Add this code cell at the beginning of the notebook and run it:

```python
# Install kaggle and download dataset
!pip install -q kaggle

# Upload your kaggle.json file when prompted
from google.colab import files
files.upload()  # Upload kaggle.json

# Setup kaggle credentials
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# Download and extract dataset
!kaggle datasets download -d alessiocorrado99/animals10
!unzip -q animals10.zip -d /content/animals10
```

**To get kaggle.json:**
1. Go to https://www.kaggle.com/settings
2. Scroll to "API" section
3. Click "Create New Token" (downloads kaggle.json)

### Step 3: Update Dataset Path

Change the dataset path in the notebook to:
```python
dataset_path = '/content/animals10/raw-img'
```

### Step 4: Run All Cells

Run the rest of the notebook normally.

## Results

- **VGG16:** 85.06% test accuracy
- **ResNet50:** 91.73% test accuracy

Full report: `CECS456_project.pdf`
