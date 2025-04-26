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
| **MobileNet** | 90.07%              | 86.24%              | 0.2960        | 0.3962          |
| **ResNet-18** | 87.27%              | 88.24%              | 0.3526        | 0.3535          |
| **ViT**       | 97.98%              | 96.11%              | 0.0663        | 0.1139          |


## Model Comparison

Across all models evaluated in this project, the Vision Transformer (ViT-B/16) achieved the highest validation accuracy of **96.11%** and the lowest validation loss of **0.1139**. 

Key observations:
- The **basic CNN** achieved a reasonable baseline accuracy of 78.09%, but was significantly outperformed by all pre-trained models.
- **AlexNet**, despite being one of the earliest deep CNN architectures, achieved strong training accuracy but had a noticeable generalization gap, with a validation accuracy of 83.44%.
- **MobileNet** showed excellent performance for a lightweight architecture, achieving 86.24% validation accuracy, balancing speed and accuracy well.
- **ResNet-18**, with its residual connections, achieved better generalization than AlexNet and MobileNet, reaching 88.24% validation accuracy.
- **ViT-B/16** surpassed all convolutional models, demonstrating the effectiveness of transformer-based architectures even without full fine-tuning.

These results highlight that transformer models, when used as feature extractors and with minimal architectural tuning, can outperform traditional CNNs in image classification tasks.

##  Training Environment

- Models were trained using **Google Colab**.
- Hardware accelerator: **NVIDIA T4 GPU** provided by Colab.
- Frameworks: TensorFlow, PyTorch, Torchvision.