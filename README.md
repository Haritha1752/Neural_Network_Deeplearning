# CelebA Face Recognition – Milestone 1

## Project Overview  
This project implements **celebrity face recognition** using the **CelebA dataset**.  
We trained multiple deep learning models (ResNet18, ResNet34, EfficientNet-B0) to classify celebrity identities in a **closed-set classification** setting.  

The goal of this milestone was to:
- Build and preprocess the dataset.
- Train CNN-based models for identity classification.
- Compare different architectures.
- Evaluate performance and save checkpoints for inference.

---

## Dataset Details  
- **Dataset**: CelebA (Aligned & Cropped Faces)  
- **Subset Used**: 40k images (closed-set split: train/val/test).  
- **Classes (IDs)**: 666 unique celebrity identities.  
- **Split Summary**:  
  - Train: ~32k images  
  - Validation: ~4k images  
  - Test: ~4k images  

---

## Models Trained  
We experimented with the following architectures:

| Model             | Best Val Accuracy | Test Accuracy | Notes |
|-------------------|------------------|---------------|-------|
| **ResNet18**      | ~0.72            | ~0.70         | Baseline, smaller model |
| **ResNet34**      | ~0.62            | ~0.61         | Deeper, but underperformed |
| **EfficientNet-B0** | **0.73**        | **0.73**      | Best performing |

---

## Proof of Model Performance  
### Training Logs (EfficientNet-B0 example):  
- Val Accuracy: **73%**  
- Test Accuracy: **72.9%**  

### Example Prediction Output:  
For a test image, the model predicts the **celebrity ID index**.

---

## Milestone Achievements  
- Dataset subset created and preprocessed.  
- Baseline (ResNet18) and advanced (EfficientNet-B0) models trained.  
- Achieved **73% accuracy** with EfficientNet-B0 on test set.  
- Inference script created to predict ID from a single test image.  
- Repository initialized and linked to GitHub.  


