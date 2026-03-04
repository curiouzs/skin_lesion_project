# Skin Lesion Project

## Skin Disease Classification Using Deep Learning

This project presents an automated image-based classification system designed for identifying different categories of skin conditions using convolutional neural networks. The system leverages transfer learning with **MobileNetV2**, a lightweight yet powerful deep learning architecture optimized for visual recognition tasks. By integrating structured data preprocessing, model training, and evaluation workflows, the framework enables efficient and scalable medical image classification.

The dataset is organized into structured class folders for training and validation, enabling supervised learning through labeled dermatological images. Images are resized to a fixed resolution (160×160) to ensure architectural compatibility and computational efficiency. Standardized preprocessing techniques are applied to maintain consistency across the data pipeline.

The model architecture is built upon the pretrained MobileNetV2 backbone, allowing extraction of high-level visual features such as texture patterns, lesion boundaries, and pigmentation variations. A custom classification head is appended to adapt the network for multi-class skin condition prediction. The training process utilizes stochastic optimization techniques to iteratively minimize classification loss and improve generalization performance.

To facilitate interpretability and evaluation, the project includes:

* Visualization of training and validation accuracy
* Class distribution analysis
* Performance monitoring across epochs
* Inference on independent test images

The system outputs predicted class labels along with confidence scores, enabling reliable decision support in dermatological image analysis contexts. The modular design allows seamless integration of additional datasets or extension to related medical image classification tasks.

### Key Features

* Transfer learning–based architecture using MobileNetV2
* Multi-class image classification framework
* Structured dataset handling with generator-based loading
* Visualization-driven performance monitoring
* Scalable and lightweight model suitable for deployment

This project demonstrates the practical application of deep learning in medical image analysis, combining computational efficiency with structured training methodology to support automated skin condition recognition.
