# Transposed Convolution & Upsampling with Bilinear Interpolation 

This repository contains hands-on exercises for **transposed convolution** and **upsampling** in neural networks. The exercises are implemented in **Google Colab** and demonstrate how to increase the resolution of images using learned convolution kernels and bilinear interpolation.

---

## Overview

In this exercise, we explore:

1. **Transposed Convolution (Deconvolution)**  
   - Used for upsampling in neural networks.
   - Examine how the kernel transforms a small matrix into a larger one.

2. **Bilinear Interpolation Upsampling**  
   - Modify the transposed convolution to mimic bilinear interpolation.
   - Compare the output matrices and visualize results on a real image.

The exercises are divided into the following steps:

- Running `tconv.py` to observe transposed convolution outputs.
- Modifying the kernel to perform bilinear interpolation.
- Applying the modified kernel to upsample an image (`upsample_im.py`).

---

## Setup

1. Open a **new Google Colab runtime**.
2. Upload the provided files from Moodle:
   - `tconv.py`
   - `upsample_im.py`
   - `example.png` (image for upsampling)
3. Run `tconv.py` to inspect the initial matrix outputs:

```python
!python tconv.py
