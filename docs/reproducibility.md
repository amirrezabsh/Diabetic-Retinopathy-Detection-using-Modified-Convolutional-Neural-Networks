# Reproducibility

## Environment

Create a fresh Python environment and install dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

The original implementation uses TensorFlow/Keras and notebook-based experimentation. GPU execution is recommended for training.

## Running the Notebook

```bash
jupyter notebook notebooks/BscProject.ipynb
```

Run cells from top to bottom. If the notebook contains paths from Google Colab or an older local environment, update them before execution.

## Recommended Experiment Record

For each serious experiment, record:

- dataset version,
- split ratios,
- preprocessing settings,
- image resolution,
- model architecture,
- optimizer and learning rate,
- batch size,
- number of epochs,
- random seed,
- final validation/test metrics.

## Artifacts

Keep large artifacts outside Git:

- trained model files,
- checkpoints,
- TensorBoard logs,
- generated predictions,
- exported datasets,
- local caches.

Use `artifacts/`, `models/`, or an external storage location for these files.

