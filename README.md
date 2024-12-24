# CNN Transfer-Learning: Fine-Tuning VGG16 on CIFAR10 dataset

## Overview

This project demonstrates how to fine-tune a powerful Convolutional Neural Network (CNN) model (VGG16) on the CIFAR10 dataset, which will demonstrate:

- **Transfer Learning**: Using a pre-trained model (VGG16) trained on ImageNet.
- **Custom Model Modification**: Replacing VGG16's final classification layers to handle CIFAR10 classes.
- **Training & Evaluation**: Training loops, validation, and plotting learning curves.
- **Practical Techniques**: Applying different learning rates and weight decay parameters to different parts of the network.

---

## Dependencies and Installation

1. **Python 3.7+**  
2. **PyTorch** and **Torchvision**  
3. **NumPy** and **Matplotlib**  
4. **scikit-learn**

---

## Dataset

I used the CIFAR10 dataset, consisting of 32x32 color images in 10 classes (e.g., airplanes, automobiles, birds, cats, etc.). The dataset will be automatically downloaded when you run the script.

---

## Results

Transfer Learning significantly speeds up convergence and can yield high accuracy compared to training from scratch. A typical run with 10 epochs (or less) can achieve reasonably good accuracy on CIFAR10 (varies by hyperparameter tuning).

**Sample training-output snippet:**

```
Epoch 0 [Train]: Loss: 0.5543 ± 0.2648, Acc: 82.20%, Time: 521.13s
Epoch 0 [Validate]: Loss: 0.4883 ± 0.1437, Acc: 84.72%, Time: 41.14s

Epoch 1 [Train]: Loss: 0.3210 ± 0.1278, Acc: 89.88%, Time: 519.66s
Epoch 1 [Validate]: Loss: 0.3531 ± 0.1198, Acc: 88.61%, Time: 41.11s

Epoch 2 [Train]: Loss: 0.2506 ± 0.1136, Acc: 92.18%, Time: 519.62s
Epoch 2 [Validate]: Loss: 0.3208 ± 0.1380, Acc: 90.15%, Time: 41.29s

Epoch 3 [Train]: Loss: 0.2142 ± 0.1170, Acc: 93.46%, Time: 519.64s
Epoch 3 [Validate]: Loss: 0.4342 ± 0.1731, Acc: 87.35%, Time: 40.98s

Epoch 4 [Train]: Loss: 0.1838 ± 0.1040, Acc: 94.46%, Time: 519.55s
Epoch 4 [Validate]: Loss: 0.2913 ± 0.1370, Acc: 91.54%, Time: 41.04s

Epoch 5 [Train]: Loss: 0.1606 ± 0.1027, Acc: 95.24%, Time: 519.54s
Epoch 5 [Validate]: Loss: 0.3136 ± 0.1397, Acc: 91.11%, Time: 41.07s

Epoch 6 [Train]: Loss: 0.1495 ± 0.1018, Acc: 95.58%, Time: 519.57s
Epoch 6 [Validate]: Loss: 0.3419 ± 0.1786, Acc: 90.22%, Time: 41.14s

Epoch 7 [Train]: Loss: 0.1328 ± 0.0926, Acc: 96.02%, Time: 519.56s
Epoch 7 [Validate]: Loss: 0.3765 ± 0.1831, Acc: 89.87%, Time: 41.09s

Epoch 8 [Train]: Loss: 0.1323 ± 0.0970, Acc: 96.12%, Time: 519.57s
Epoch 8 [Validate]: Loss: 0.3724 ± 0.1843, Acc: 90.33%, Time: 41.12s

Epoch 9 [Train]: Loss: 0.1128 ± 0.0897, Acc: 96.74%, Time: 519.54s
Epoch 9 [Validate]: Loss: 0.3497 ± 0.1854, Acc: 90.80%, Time: 41.14s
```

---

## Contributing

If you'd like to contribute to this project, feel free to open an issue or submit a pull request with improvements or bug fixes.
