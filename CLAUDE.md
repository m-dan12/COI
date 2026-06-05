# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

University lab course: **Цифровая обработка изображений** (Digital Image Processing), Samara University. Labs are implemented as Jupyter Notebooks in Python.

## Requirements & Student Info

See `ТРЕБОВАНИЯ.md` for full requirements: student name/group, notebook naming, report structure, model assignments per lab, and special notes.

## Lab Assignment Files

- `Лабораторная работа 1.md` — Image capture (webcam), color spaces (GrayScale/HSV/LAB/YCrCb), gamma correction, histogram equalization
- `Лабораторная работа 2.md` — Debayerization: nearest-neighbor, superpixel, bilinear vs bicubic interpolation, Malvar-He-Cutler algorithm
- `Лабораторная работа 3.md` — White balance correction: gray card, brightest-region, Gray World algorithm, color temperature (Kelvin)

## Notebook Naming Convention

```
<group_number>-090401D-<LastNameFirstNamePatronymic>-ЛР<lab_number>.ipynb
```

## Notebook Structure Requirements

Each lab notebook must follow this cell order:
1. Title cell (markdown) — author info and lab description
2. For each task: task text (markdown) → code cell → output cells (images/values) → optional commentary (markdown)

## Common Libraries

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
from skimage.metrics import peak_signal_noise_ratio as psnr
from skimage.metrics import structural_similarity as ssim
```

## Running Notebooks

```bash
jupyter notebook
# or
jupyter lab
```

Run a specific notebook non-interactively:
```bash
jupyter nbconvert --to notebook --execute <notebook_name>.ipynb
```
