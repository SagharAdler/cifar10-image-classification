# cifar10-image-classification

This project contains implementations, fine-tuning, and linear probing of various deep learning models for image classification on the CIFAR-10 dataset. Models include a **custom CNN**,  **AlexNet**, **MobileNet**, **ResNet-18**, and **Vision Transformer (ViT)**.

Each model is trained and evaluated on CIFAR-10, which consists of 60,000 32x32 color images across 10 classes. The aim is to compare performance across different model architectures, from traditional CNNs to modern transformer-based models.

---

##  Models Used

- `CNN`: A simple custom convolutional network trained from scratch.
- `AlexNet`: Classical CNN architecture, adapted for CIFAR-10.
- `MobileNet`: Lightweight model optimized for speed and low memory.
- `ResNet-18`: Residual learning-based deep CNN.
- `ViT`: Vision Transformer using self-attention instead of convolutions.

---

##  Model Performance

| Model         | Training Accuracy | Validation Accuracy | Training Loss | Validation Loss |
|---------------|--------------------|---------------------|---------------|-----------------|
| **CNN**       | 80.26%              | 78.09%              | 0.6391        | 0.5613          |
| **AlexNet**   | 96.14%              | 83.44%              | 0.1496        | 0.5394          |
| **MobileNet** | *TBD*               | *TBD*               | *TBD*         | *TBD*           |
| **ResNet-18** | *TBD*               | *TBD*               | *TBD*         | *TBD*           |
| **ViT**       | *TBD*               | *TBD*               | *TBD*         | *TBD*           |



##  Training Environment

- Models were trained using **Google Colab**.
- Hardware accelerator: **NVIDIA T4 GPU** provided by Colab.
- Frameworks: TensorFlow, Pandas, Matplotlib.