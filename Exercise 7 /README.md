# Camera Calibration Using a Checkerboard Pattern

## Overview
This exercise performs **camera calibration** using images captured with a personal
smartphone camera. The goal is to estimate the **intrinsic camera parameters**, including
the **camera intrinsic matrix K**, using a planar checkerboard calibration pattern.

Calibration is implemented in **Python using OpenCV** and executed in **Google Colab**.

## Requirements
- Python 3
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- Google Colab
- 
## Files
- `calibrate-camera.ipynb` – Camera calibration notebook  
- `calibration-pattern.pdf` – Checkerboard calibration pattern  
- `checkerboard0-200x155.jpg` – Calibration image (view 1)  
- `checkerboard1-156x200.jpg` – Calibration image (view 2)  
- `checkerboard2-156x200.jpg` – Calibration image (view 3)  
- `README.md` – Exercise documentation  

## Checkerboard Configuration
- Inner corners: **6 × 9**
- Pattern is displayed fullscreen on a monitor
- Images are captured from different viewing angles at similar distance

```python
CHECKERBOARD = (6, 9)
