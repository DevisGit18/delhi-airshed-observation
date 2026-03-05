# SRIP 2026 - Earth Observation: Delhi Airshed Land Use Classification

## Dataset
- Source: Sentinel-2 RGB patches (128x128px, 10m/pixel), ESA WorldCover 2021
- Region: Delhi-NCR (EPSG:4326)

## Results

| Task | Result |
|---|---|
| Total images before filtering | 9216 |
| Images inside Delhi-NCR | 8015 |
| Train set (60%) | 4809 |
| Test set (40%) | 3206 |
| Model | ResNet18 (Transfer Learning) |
| Test Accuracy | 88.68% |
| F1-Score (weighted) | 0.8827 |
| F1-Score (macro) | 0.4758 |

## Per-class F1

| Class | F1-Score |
|---|---|
| Cropland | 0.94 |
| Built-up | 0.83 |
| Vegetation | 0.61 |
| Water | 0.00 |
| Others | 0.00 |

## Stack
Python, GeoPandas, Rasterio, PyTorch, ResNet18, Scikit-learn

## Disclosure
AI tools (Claude) were used as a coding assistant. All code is fully understood and can be explained during the one-on-one evaluation.
