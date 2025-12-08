# CECS 456 Deep Learning Project

**Authors:** Melody Gatan & Matthew Nguyen  
**Course:** CECS 456 - Deep Learning  
**Date:** December 5, 2025

Comparison of VGG16 and ResNet50 architectures on Animals10 dataset.

## How to Run

1. Open `VGG16_Animals10.ipynb` or `RestNet.ipynb` in Google Colab
2. Change runtime to GPU: `Runtime` → `Change runtime type` → Select `T4 GPU` or `A100 GPU`
3. Run the first cell to download the dataset (you'll need to upload your `kaggle.json` file)
   - Get kaggle.json from: https://www.kaggle.com/settings → API → "Create New Token"
4. Run all remaining cells

## Results

- **VGG16:** 85.06% test accuracy
- **ResNet50:** 91.73% test accuracy

Full report: `CECS456_project.pdf`
