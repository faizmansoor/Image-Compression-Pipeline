# Enhanced Image Compression Pipeline

A Python-based image compression pipeline implemented in a Jupyter Notebook, combining **Discrete Wavelet Transform (DWT)**, **K-Means clustering**, and **Arithmetic Coding** for efficient grayscale image compression.

This pipeline allows you to compress images, store them in a lightweight format, and decompress them while preserving visual quality. It also provides metrics like **PSNR** and **SSIM** to evaluate compression quality.

---

## Features

- **Discrete Wavelet Transform (DWT):** Reduces image redundancy in frequency space.
- **K-Means Clustering:** Reduces color intensity variations, lowering data size.
- **Arithmetic Coding:** Efficient entropy coding for further compression.
- **Quality Metrics:** Computes PSNR and SSIM for compressed vs decompressed images.
- **Visualization:** Displays images at each compression stage (original → DWT → clustered → decompressed).
- **Pickle-based Storage:** Saves compressed data as `.pkl` files for easy sharing and decompression.

---

## Installation

```bash
git clone https://github.com/faizmansoor/Image-Compression-Pipeline.git
cd image-compression-pipeline
pip install -r requirements.txt
```

##Usage

Compress and Decompress an Image

```bash
from compression_pipeline import compress_and_decompress_image
```

# Compress and decompress a grayscale image

```bash
result = compress_and_decompress_image("test-images/test1.png")
```

This will:

Save the compressed file as test1_compressed.pkl

Save the decompressed image as test1_decompressed.png

Display images at all stages

Print PSNR, SSIM, and compression ratio


## Compression Ratios:

Sample 1: 11.27:1 (91.1% size reduction)

Sample 2: 11.23:1 (91.1% size reduction)

Sample 3: 10.38:1 (90.4% size reduction)

Average Compression Ratio: 10.96:1 (~90.9% size reduction)




# Images
<img width="1116" height="405" alt="image" src="https://github.com/user-attachments/assets/775140f0-2afb-46b5-89c4-ea6e3792377e" />

<br>
<br>

<img width="1098" height="365" alt="image" src="https://github.com/user-attachments/assets/0fc6df8b-35f3-4501-90ed-f3b0e6e4fbc7" />

