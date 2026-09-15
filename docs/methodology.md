# Methodology

## Problem

The task is image classification for diabetic retinopathy screening. Given a retinal fundus image, the model predicts the retinopathy severity class.

## Approach

The notebook follows a deep-learning workflow:

1. Load image metadata and labels.
2. Load and preprocess retinal images.
3. Resize images to a consistent input shape.
4. Apply augmentation where needed.
5. Define CNN-based models.
6. Explore transfer learning with pretrained computer-vision backbones.
7. Train models on the training split.
8. Monitor validation metrics and visualize training behavior.

## Model Components

The notebook includes experiments with:

- custom convolutional layers,
- dense classification heads,
- batch normalization,
- dropout,
- transfer-learning backbones,
- hyperparameter-tuning utilities.

## Evaluation

Tracked metrics include loss, accuracy, precision, and recall. For a final thesis-grade report, also include a confusion matrix and class-wise metrics because diabetic retinopathy datasets are commonly imbalanced.

## Limitations

This repository keeps the original notebook workflow. It is clear enough for review, but not yet a fully packaged machine-learning library. A production-grade version should split preprocessing, training, evaluation, and configuration into separate modules.

