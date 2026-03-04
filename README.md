# Skin Lesion Project

## Skin Disease Classification Using Deep Learning

This project presents an automated image-based classification system for identifying multiple categories of skin conditions using deep learning techniques. The framework is built upon MobileNetV2, a computationally efficient convolutional neural network architecture designed for high-performance image recognition tasks. By combining structured dataset management, transfer learning, and systematic evaluation, the system enables scalable and reliable dermatological image analysis.

### Dataset Source

The dataset used in this project is derived from the Skin Cancer MNIST: HAM10000 dataset, originally published by the Department of Dermatology at the Medical University of Vienna and available through the Harvard Dataverse platform. The dataset is widely used in academic research for benchmarking skin lesion classification algorithms.

It contains dermatoscopic images of common pigmented skin lesions collected from multiple populations and imaging conditions. The dataset is curated to support multi-class classification tasks in medical image analysis.

### Data Description

The dataset consists of high-resolution RGB dermatoscopic images categorized into distinct diagnostic classes. Each image represents a specific type of skin lesion. The primary categories include:

Melanocytic nevi

Melanoma

Benign keratosis-like lesions

Basal cell carcinoma

Actinic keratoses

Vascular lesions

Dermatofibroma

Each image is labeled according to expert clinical diagnosis. The dataset exhibits natural class variability, reflecting realistic clinical distribution patterns.

### Data Preprocessing and Division

To ensure compatibility with the model architecture, all images are resized to 160 × 160 pixels and processed using MobileNetV2-specific normalization techniques. The dataset is organized into a directory-based structure, enabling efficient supervised learning through generator-based data loading.

The dataset is divided into:

Training Set – Used for model learning and weight optimization

Validation Set – Used for performance monitoring and generalization assessment

The split maintains representation across all classes to preserve distribution consistency during training and evaluation.

### Model Architecture

The system utilizes MobileNetV2 as a pretrained backbone for feature extraction. This architecture is selected due to its depthwise separable convolution structure, which reduces computational cost while preserving representational power. A customized classification layer is appended to adapt the network for multi-class lesion identification.

Transfer learning allows the model to leverage previously learned visual representations such as texture gradients, color distributions, and structural lesion patterns, enhancing diagnostic discrimination.
