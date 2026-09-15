# Dataset Guide

## Expected Data

The project is designed for diabetic retinopathy classification from retinal fundus images. The notebook expects:

- a directory containing retinal image files,
- a CSV file containing image identifiers and labels,
- labels representing diabetic retinopathy severity classes.

The original notebook references train/validation arrays created from image data and labels. Keep the image-label mapping stable when rerunning experiments.

## Recommended Local Layout

The dataset is intentionally excluded from Git. Use a local structure similar to:

```text
data/
├── raw/
│   ├── train_images/
│   └── train_labels.csv
└── processed/
```

If the notebook uses absolute paths from Google Colab or a local machine, update them to point to your local `data/` directory before running.

## Data Handling

Do not commit:

- raw medical images,
- generated resized images,
- model checkpoints,
- exported datasets,
- local experiment artifacts.

These files are ignored by `.gitignore`.

## Reproducibility Checklist

Before publishing results, record:

- dataset name and version,
- number of images used,
- train/validation/test split strategy,
- image size after preprocessing,
- label mapping,
- random seed,
- evaluation metrics.

