# Task 2: Transfer Learning using VGG16

**Course:** MSc DSBDA  
**Student Name:** Sharon Thoppil  
**Roll No:** 41  

## 📌 Project Overview
This project implements Transfer Learning using a pre-trained **VGG16** architecture on the **CIFAR-10** dataset (resized to 96x96 resolution). It evaluates the performance gains of feature extraction and fine-tuning over a custom baseline CNN built from scratch.

## 📊 Performance Summary
| Model Architecture | Validation Accuracy | Training Time | Accuracy Improvement |
| :--- | :---: | :---: | :---: |
| **Baseline CNN (Scratch)** | 55.95% | 25.84s | Baseline |
| **VGG16 (Feature Extractor)** | 70.50% | 97.88s | +14.55% |
| **VGG16 (Fine-Tuned)** | **75.65%** | 56.00s | **+19.70%** |

## 🚀 Key Takeaways
1. **Transfer Learning Efficiency:** Freezing pre-trained ImageNet layers improved accuracy by **+14.55%** over the baseline CNN without updating base weights.
2. **Fine-Tuning Impact:** Unfreezing the final convolutional block (`block5`) with a lower learning rate ($10^{-4}$) yielded the highest overall accuracy (**75.65%**).

## 📁 Repository Structure
