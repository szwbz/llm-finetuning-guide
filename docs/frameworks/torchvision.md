# torchvision Guide

## Frameworks Overview

torchvision is a popular computer vision library for PyTorch that provides datasets, model architectures, and image transformations. Current version: 0.25.0 (Released: 2026-01-06)

### Key Features
- Pre-trained models (ResNet, EfficientNet, Vision Transformer)
- Dataset utilities (ImageNet, CIFAR, etc.)
- Image transformations and augmentations
- Video processing utilities

### Installation
```bash
pip install torchvision
```

### Basic Usage
```python
import torchvision
import torchvision.transforms as transforms

# Load dataset
transform = transforms.Compose([
    transforms.Resize(256),
    transforms.CenterCrop(224),
    transforms.ToTensor(),
])
```

### Best Practices
- Use torchvision.transforms for data augmentation
- Leverage pre-trained models for transfer learning
- Batch normalization and proper normalization values