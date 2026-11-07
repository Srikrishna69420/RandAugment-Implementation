# RandAugment implementation

A notebook-based implementation and CIFAR-10 experiment inspired by the RandAugment paper. The notebook defines the augmentation operations and magnitude mapping, composes RandAugment with a WideResNet training pipeline, and records experiment observations.

## Quick start

Open `RandAugment.ipynb` in Jupyter or Google Colab and run the cells in order.

```bash
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows PowerShell: .venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
jupyter notebook RandAugment.ipynb
```

A CUDA-capable GPU is recommended for the full training run.

## Layout

- `RandAugment.ipynb` — canonical implementation, training pipeline, and observations.
- `docs/REPRODUCIBILITY.md` — setup and experiment details.
- `requirements.txt` — Python dependencies.

## Main experiment settings

The notebook exposes the number of operations and augmentation magnitude in its configuration. It records a WideResNet-28-10 CIFAR-10 experiment and reports its own settings and observed accuracy. These are the notebook's reported results, not an independent verification or a compute-matched reproduction of the paper.

## Data

CIFAR-10 is downloaded by torchvision into `./data` when the notebook is run.

