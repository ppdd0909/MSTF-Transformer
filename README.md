# MSTF-Transformer
Multi-modal Spatio-temporal Feature Fusion for Building Occupancy Prediction

> ⚠️ Full training code will be released upon acceptance of the manuscript.  
> This repository provides hyperparameter configurations and result figures for transparency and reproducibility.

## Environment

| OS | macOS 15.7.3 (arm64) |
| Hardware | Apple M4 CPU, Apple MPS (Metal Performance Shaders) |
| Python | 3.12.7 |
| PyTorch | 2.6.0 |
| Key Libraries | numpy, pandas, matplotlib |

> No CUDA/CuDNN required. The code is compatible with CPU and Apple MPS.

## Model Configuration

Full hyperparameters are provided in `config.yaml`. 

## Multi-modal Feature Decoupling

Input features are decoupled into three modalities based on physical semantics:

| M1 — Personnel Dynamics | F1 | Historical Occupant Number |
| M2 — Environmental State | F2, F3, F4, F5 | Room Temp 1, Room RH 1, Room Temp 2, Room RH 2 |
| M3 — Equipment Control | F6, F7, F8, F9 | FCU Temp Feedback, FCU Control Mode, FCU On/Off, FCU Fan |


## Dataset

**Public dataset:**
> Kailai Sun et al., *Building occupancy number prediction: A Transformer approach*, Building and Environment, 244, 2023, 110807.

**Real-world validation dataset:**
- Office building (educational use), Anhui, China (May 19–30, 2025)
- Raw data not included due to privacy constraints


## Repository Contents

| `config.yaml` | Full hyperparameter configuration |
| `figures/loss_curve.png` | Training loss curve across epochs |
| `figures/error_histogram.png` | Prediction error distribution histogram |
| `figures/confusion_matrix_zone7.png` | Confusion matrix for Zone 7 |

## Citation

Citation information will be provided upon acceptance.
