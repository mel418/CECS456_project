# CECS 456 Deep Learning Project

**Authors:** Melody Gatan & Matthew Nguyen  
**Course:** CECS 456 - Deep Learning  
**Date:** December 5, 2025

Comparison of VGG16 and ResNet50 architectures on Animals10 dataset.

## How to Run

### Step 1: Get the Dataset

**Option 1 (For Professor):**
1. Add the shared `CECS456_Project` folder to your Google Drive
2. Right-click the shared folder → "Add shortcut to Drive"

**Option 2 (Manual Download):**
1. Download Animals10 dataset from Kaggle: https://www.kaggle.com/datasets/alessiocorrado99/animals10
2. Upload to your Google Drive at: `CECS456_Project/raw-img/`

### Step 2: Run the Notebooks

1. Open `VGG16_Animals10.ipynb` or `RestNet.ipynb` in Google Colab
2. Change runtime to GPU: `Runtime` → `Change runtime type` → Select `T4 GPU` or `A100 GPU`
3. Run all cells

**Note:** Dataset path is set to `/content/drive/MyDrive/CECS456_Project/raw-img`

## Results

- **VGG16:** 85.06% test accuracy
- **ResNet50:** 91.73% test accuracy

Full report: `CECS456_project.pdf`
