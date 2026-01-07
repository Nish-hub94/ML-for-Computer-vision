# Harris and SIFT Feature Detection and Matching

## Overview
This project explores **classical feature detection and matching techniques** in computer vision.
We begin with **Harris corner detection**, proceed to **SIFT feature detection**, and finally build a
robust **feature matching pipeline** between two images using **brute-force matching** and
**k-Nearest Neighbors (kNN) with Lowe’s ratio test**.

All experiments are implemented in **Python using OpenCV** and executed in **Google Colab**.

---

## Requirements
- Python 3
- OpenCV (`cv2`)
- NumPy
- Matplotlib

---

## Files
- `ref1.png` – Reference image  
- `rot1.png` – Rotated version of the reference image  
- `harris-corners.py` – Harris corner detection implementation  
- `sift-detector.py` – SIFT detection and feature matching code  
- `README.md` – Project documentation  

---

## 1. Harris Corner Detection

### Description
The Harris corner detector identifies points in an image where intensity variations occur
strongly in both horizontal and vertical directions.

### Implementation
The OpenCV function used is:

