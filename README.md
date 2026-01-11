# K-Means Image Compression (16-colour palette) using NumPy (from scratch)

A simple notebook that compresses an RGB image by clustering pixels in **RGB space** using a **from-scratch K-Means** implementation (NumPy).  
Each pixel is replaced by its nearest centroid colour, yielding a reduced **16-colour palette** while preserving the overall appearance.

## Approach
- **Input:** RGB image of shape (H, W, 3)
- **Representation:** each pixel is a data point \(x = (R, G, B)\)
- **Algorithm:** K-Means clustering
- **K:** 16 (palette size)
- **Output:** compressed image where each pixel is mapped to its closest centroid

## How to run
```bash
pip install -r requirements.txt
jupyter notebook notebook/kmeans_image_compression.ipynb
```

## Notes

For large images, the from-scratch K-Means (Python loops) can be slow.
If needed, resize the image (e.g. 128×128 or 256×256) before running K-Means.
