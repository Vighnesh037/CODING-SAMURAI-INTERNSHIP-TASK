# Image Classification Using Transfer Learning

## Overview

This project implements an image classification model using **Transfer Learning** with **MobileNetV2**. The model classifies hand gesture images into three categories: **Rock**, **Paper**, and **Scissors**. By leveraging a pre-trained convolutional neural network, the model achieves high accuracy while requiring only a small amount of training.

---

## Objective

The objective of this project is to build an efficient image classification system using a pre-trained deep learning model and evaluate its performance on a custom image dataset.

---

## Dataset

* **Dataset:** Rock-Paper-Scissors Image Dataset
* **Total Images:** 2,188
* **Classes:** Rock, Paper, Scissors
* **Image Size:** 300 × 200 pixels (resized to 224 × 224 for training)

> **Note:** The dataset is not included in this repository due to its size. It can be downloaded from the original source:
> https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors

---

## Technologies Used

* Python
* TensorFlow
* Keras
* MobileNetV2
* NumPy
* Matplotlib

---

## Model Architecture

* MobileNetV2 (Pre-trained on ImageNet)
* Image Rescaling Layer
* Global Average Pooling Layer
* Dense Layer (128 Units, ReLU)
* Dropout Layer (0.3)
* Output Layer (Softmax)

---

## Training Configuration

* Image Size: **224 × 224**
* Batch Size: **32**
* Validation Split: **20%**
* Optimizer: **Adam**
* Loss Function: **Sparse Categorical Crossentropy**
* Epochs: **5**

---

## Results

| Metric              |      Value |
| ------------------- | ---------: |
| Training Accuracy   | **99.83%** |
| Validation Accuracy | **99.54%** |
| Validation Loss     | **0.0090** |

The model achieved excellent classification performance while maintaining a very small gap between training and validation accuracy, indicating good generalization.

---

## Sample Prediction

The trained model successfully predicts unseen images with high confidence.

Example:

* **Prediction:** Paper
* **Confidence:** 99.92%

---




---

## How to Run

1. Clone this repository.
2. Download the Rock-Paper-Scissors dataset.
3. Install the required libraries:

```bash
pip install tensorflow matplotlib numpy pillow scikit-learn
```

4. Update the dataset path in the notebook.
5. Run all notebook cells to train and evaluate the model.

---

## Future Improvements

* Fine-tune the MobileNetV2 base model.
* Train on a larger and more diverse dataset.
* Develop a real-time webcam-based Rock-Paper-Scissors classifier.

---

## Conclusion

This project demonstrates the effectiveness of **Transfer Learning** for image classification tasks. Using a pre-trained MobileNetV2 model significantly reduced training time while achieving a validation accuracy of **99.54%**. The project highlights the practical application of deep learning for image recognition problems.
