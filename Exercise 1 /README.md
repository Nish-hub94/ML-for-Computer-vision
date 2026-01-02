# Exercise 1 – Introduction to Google Colab and Basic Image Handling

## Overview
In this exercise, we learn to use **Google Colab**, explore basic **computer vision libraries**, and understand how **images are represented in memory**.  
The main goal is to manipulate and visualize images using Python libraries like **OpenCV**, **Matplotlib**, and **NumPy**.

---

## Topics Covered
- Setting up and using **Google Colab**
- Uploading files to Colab
- Reading and displaying images with **OpenCV** (`cv2`) and **Matplotlib**
- Understanding image representation in memory (`NumPy` arrays)
- Accessing and modifying pixel values
- Memory usage of images
- Basic pixel arithmetic and image manipulation
- Rotating images using Python `for` loops

---

## Step-by-Step Instructions

1. **Open Google Colab**  
   - Go to [colab.google.com](https://colab.google.com) and create a new notebook in your Drive.

2. **Upload the example image**  
   - Fetch `example.png` from the course Moodle page.
   - Upload it to Colab using the left-hand panel (Files → Upload).

3. **Display the image**  

```python
import cv2
from matplotlib import pyplot as plt

img_bgr = cv2.imread('example.png', cv2.IMREAD_COLOR)
img_rgb = cv2.cvtColor(img_bgr, cv2.COLOR_BGR2RGB)

plt.imshow(img_rgb)
plt.axis("off")
plt.show()
