# VGG16 Animal Classification - Animals10 Dataset

## 👤 Author
**Melody Gatan** - VGG16 Implementation

## 📊 Project Overview
Implementation of VGG16 Convolutional Neural Network for classifying 10 different animal species.

## 🎯 Dataset
- **Source**: Animals10 from Kaggle
- **Total Images**: 26179
- **Classes**: 10 (cane, cavallo, elefante, farfalla, gallina, gatto, mucca, pecora, ragno, scoiattolo)
- **Split**: 
  - Training: 18325 images (70%)
  - Validation: 3926 images (15%)
  - Test: 3928 images (15%)

## 🏗️ Model Architecture
- **Base Model**: VGG16 (pre-trained on ImageNet)
- **Total Parameters**: 134,301,514
- **Trainable Parameters**: 119,586,826
- **Input Size**: 224×224×3
- **Modifications**: 
  - Froze convolutional layers
  - Modified final fully connected layer for 10 classes
  - Added dropout for regularization

## 📈 Results
- **Test Accuracy**: 94.65%
- **Best Validation Accuracy**: 94.93%
- **Training Time**: 6.41 minutes
- **Best Performing Class**: ragno (98.73%)
- **Most Challenging Class**: pecora (88.85%)

## 🛠️ Training Configuration
- **Epochs**: 10
- **Batch Size**: 64
- **Learning Rate**: 0.001
- **Optimizer**: Adam
- **Loss Function**: Cross-Entropy
- **Device**: cuda

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
1. VGG16 achieved 94.65% accuracy on Animals10 dataset
2. Training converged in 10 epochs
3. Best performing class: ragno
4. Most confused classes can be seen in confusion matrix

---
*Generated on Google Colab with T4 GPU*
