# 🍅 TomatoDiseaseNet

## Overview

**TomatoDiseaseNet** is a Convolutional Neural Network (CNN) developed to classify tomato leaf diseases from images. The model uses multiple convolutional and pooling layers to extract visual features and predict one of **10 disease classes**.
This project demonstrates practical deep learning for agricultural disease detection.

---

## Model Architecture

* 3 Convolutional Layers (Conv2D)
* ReLU Activation
* MaxPooling Layers
* Flatten Layer
* Fully Connected (Dense) Layers
* Dropout for regularization
* Output Layer: 10 classes

**Framework:** PyTorch

---

## Dataset

The model is trained on a tomato leaf disease image dataset containing labeled images of healthy and diseased leaves.

**Classes:**

* Healthy
* Bacterial Spot
* Early Blight
* Late Blight
* Leaf Mold
* Septoria Leaf Spot
* Spider Mites
* Target Spot
* Mosaic Virus
* Yellow Leaf Curl Virus

---

## Training

* Loss Function: CrossEntropyLoss
* Optimizer: Adam
* Epochs: (set by user)
* Device: CPU / GPU

Random seeds are fixed for reproducibility:

```python
torch.manual_seed(42)
torch.cuda.manual_seed(42)
```

---

## Usage

```python
loss_value = train_epoch(
    model,
    optimizer,
    lossfn,
    train_loader,
    device="cuda"
)
```

---

## Goal

To build a reliable deep learning model that can assist in **early detection of tomato plant diseases** using image classification.

---

## Future Improvements

* Add Batch Normalization
* Use Transfer Learning (ResNet / EfficientNet)
* Data Augmentation
* Deploy as a web or mobile application
* Improve accuracy and generalization

---

## Author

Shirsha Nag | Quantum & ML developer

Developed as a deep learning project for **image classification and agricultural AI applications**.
