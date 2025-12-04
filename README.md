# VGG16 Animal Classification - Animals10 Dataset

## 👤 Author
**Melody Gatan** - VGG16 Implementation

## 📊 Project Overview
Implementation of VGG16 Convolutional Neural Network for classifying 10 different animal species.

## 🎯 Dataset
- **Source**: Animals10 from Kaggle
- **Total Images**: {len(full_dataset)}
- **Classes**: {len(class_names)} ({', '.join(class_names)})
- **Split**: 
  - Training: {len(train_dataset)} images (70%)
  - Validation: {len(val_dataset)} images (15%)
  - Test: {len(test_dataset)} images (15%)

## 🏗️ Model Architecture
- **Base Model**: VGG16 (pre-trained on ImageNet)
- **Total Parameters**: {total_params:,}
- **Trainable Parameters**: {trainable_params:,}
- **Input Size**: 224×224×3
- **Modifications**: 
  - Froze convolutional layers
  - Modified final fully connected layer for 10 classes
  - Added dropout for regularization

## 📈 Results
- **Test Accuracy**: {test_accuracy:.2f}%
- **Best Validation Accuracy**: {max(history['val_acc']):.2f}%
- **Training Time**: {training_time/60:.2f} minutes
- **Best Performing Class**: {vgg_summary['best_class']} ({vgg_summary['best_class_accuracy']:.2f}%)
- **Most Challenging Class**: {vgg_summary['worst_class']} ({vgg_summary['worst_class_accuracy']:.2f}%)

## 🛠️ Training Configuration
- **Epochs**: {EPOCHS}
- **Batch Size**: {BATCH_SIZE}
- **Learning Rate**: {LEARNING_RATE}
- **Optimizer**: Adam
- **Loss Function**: Cross-Entropy
- **Device**: {device}

## 📦 Requirements
```
torch>=1.9.0
torchvision>=0.10.0
matplotlib>=3.3.0
scikit-learn>=0.24.0
pillow>=8.0.0
numpy>=1.19.0
seaborn>=0.11.0
tqdm>=4.62.0
```

## 🚀 How to Run in Google Colab
1. Open the notebook in Colab
2. Enable GPU: Runtime → Change runtime type → GPU
3. Mount Google Drive
4. Upload kaggle.json for dataset download
5. Run all cells sequentially

## 📁 Project Structure
```
CECS456_Project/
├── vgg16_animals10_classification.ipynb
├── vgg16_animals10.pth (saved model)
├── vgg16_training_curves.png
├── vgg16_confusion_matrix.png
├── vgg16_per_class_accuracy.png
├── vgg16_complete_results.txt
└── README.md
```

## 📝 Key Findings
1. VGG16 achieved {test_accuracy:.2f}% accuracy on Animals10 dataset
2. Training converged in {EPOCHS} epochs
3. Best performing class: {vgg_summary['best_class']}
4. Most confused classes can be seen in confusion matrix

---
*Generated on Google Colab with T4 GPU*
