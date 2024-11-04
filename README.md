## Overview
This analysis benchmarks a standard VGG19 model against custom variations incorporating additional layers and transformations on the Open Images dataset, comparing their classification performance.
## Key Components
### Base Model: VGG19
- Standard architecture
- Three-class classification (Frog, Fish, Bird)
- 70/30 train/test split

### Model Variations
- Randomly initialized VGG19
- ImageNet pre-trained VGG19
- Custom VGG19 with inception layer modifications

### Optimization Techniques
- Transfer learning
- Data cleansing

### Data augmentation:
- Random flip
- Random contrast
- Random translation

### Architectural Modifications
- Inception layer after block4_conv4
- Additional convolutional layers:
- 1x1 conv (1024 filters, leaky ReLU)
- 3x3 conv (1024 filters, ReLU)
- Selective layer freezing

### Evaluation Metrics
- Train vs. test accuracy
- Inference time
- Model parameters
- Confusion matrix
- Activation map analysis

## Environment
- This notebook was developed in Kaggle hence some details might need to be adjusted for local development
