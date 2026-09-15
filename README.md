# Diabetic Retinopathy Detection Using Modified CNNs

Bachelor thesis project for diabetic retinopathy severity classification from retinal fundus images using convolutional neural networks and transfer learning.

## Project Summary

Diabetic retinopathy is a diabetes-related eye disease that can cause vision loss when it is not detected early. This project explores deep-learning based image classification for diabetic retinopathy screening, with a focus on CNN architectures, transfer learning, image preprocessing, augmentation, and model evaluation.

The repository currently preserves the original thesis notebook and adds a clean project structure around it so the work is easier to review, reproduce, and extend.

## Repository Structure

```text
.
├── docs/
│   ├── dataset.md
│   ├── methodology.md
│   └── reproducibility.md
├── notebooks/
│   ├── BscProject.ipynb
│   └── README.md
├── .gitignore
├── README.md
└── requirements.txt
```

## Main Notebook

The main implementation is available in:

- [`notebooks/BscProject.ipynb`](notebooks/BscProject.ipynb)

The notebook includes data loading, preprocessing, augmentation, CNN model definitions, transfer-learning experiments, model training, and metric visualization.

## Technical Scope

- Retinal fundus image classification
- Diabetic retinopathy severity prediction
- CNN-based feature extraction
- Transfer learning with pretrained computer-vision backbones
- Data augmentation and image resizing
- Training/validation split handling
- Accuracy, loss, precision, and recall tracking

## Dataset

The notebook expects retinal image files and a label CSV. The dataset itself is not stored in this repository because medical-image datasets are large and may have licensing or privacy constraints.

See [`docs/dataset.md`](docs/dataset.md) for the expected dataset layout.

## Setup

Use Python 3.8+ with a virtual environment.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Then open the notebook:

```bash
jupyter notebook notebooks/BscProject.ipynb
```

## Reproducibility Notes

This repository is based on an academic notebook workflow. For reproducible reruns, keep the dataset layout stable, record the dataset source/version, and run the notebook from top to bottom in a clean environment.

More details are documented in [`docs/reproducibility.md`](docs/reproducibility.md).

## Project Status

This repository represents the thesis implementation and experiment record. It is suitable for academic review and portfolio presentation, but further production hardening would require:

- separating reusable model and preprocessing code from the notebook,
- adding automated tests for preprocessing utilities,
- adding experiment configuration files,
- storing trained model artifacts outside Git,
- tracking experiments with a tool such as MLflow, Weights & Biases, or a structured results table.

## License

No open-source license has been selected yet. Add a license before reusing or distributing the project beyond academic review.
