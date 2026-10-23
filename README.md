# OpenCV Image Processing

A small image-processing assignment demonstrating common **OpenCV** operations applied to a single image, each displayed side-by-side with the original using Matplotlib.

## Operations covered

| Operation | Method |
|-----------|--------|
| Brightness & contrast | `cv2.addWeighted` and `cv2.convertScaleAbs` (α·f + β) |
| Sharpening | custom 3×3 kernel via `cv2.filter2D` |
| Sharpening (Laplacian) | `cv2.Laplacian` |
| Denoising — median | `cv2.medianBlur` |
| Denoising — Gaussian | `cv2.GaussianBlur` |
| Color enhancement | hue/saturation/value scaling in HSV space |
| Resizing | `cv2.resize` |
| Color inversion | `255 - image` |

Each cell loads the image, applies one operation, saves the result as a `.jpg`, and plots the before/after.

## Input image

The notebook reads a single image from `/content/sunflower.png` (Colab path). Drop your own image there, or change the path in each cell to point at your file. The image is **not** included in this repository.

## Requirements

- `opencv-python`
- `numpy`
- `matplotlib`

Install everything with:

```bash
pip install -r requirements.txt
```

## Getting started

1. Open the notebook in Jupyter or Google Colab.
2. Place an image at the path used in the cells (`/content/sunflower.png`) or update the path.
3. Run the cells top to bottom — each produces a saved output image and a before/after plot.

## Repository structure

```
.
├── Pic_Assignment.ipynb
└── README.md
```

## License

Add a license of your choice (e.g. MIT) if you want others to reuse this work.
