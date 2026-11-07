# Reproducibility notes

## Run order

Run all cells in `RandAugment.ipynb` sequentially. The notebook includes augmentation functions, the RandAugment transform, WideResNet, configuration, CIFAR-10 data loaders, optimizer/scheduler, training, and reported observations.

## Dataset

The notebook uses `torchvision.datasets.CIFAR10` with `download=True` and stores the dataset in `./data`, relative to the notebook kernel's working directory.

## Environment

Install dependencies from `requirements.txt`. The notebook uses PyTorch, torchvision, NumPy, and Pillow. A CUDA-compatible GPU is recommended. Install the PyTorch/torchvision pair appropriate for your platform and CUDA runtime.

## Parameters and reported results

The notebook defines the operation count and magnitude in its configuration. It also records epoch counts, runtime, and observed test accuracy. Preserve those values when documenting a run; do not compare runs unless data split, seed, hardware, software versions, and all hyperparameters are controlled.

## Repeatability and outputs

The notebook sets some run parameters directly in cells. Record the exact configuration and software versions for future comparisons. Any generated checkpoints, logs, or plots should be stored separately and committed only when intentionally curated.
