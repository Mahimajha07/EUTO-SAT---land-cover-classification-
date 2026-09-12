# EuroSAT Land Cover Classification & SAR-to-Optical Image Translation 🛰️

This repo contains two satellite imagery deep learning projects:

1. **Land Cover Classification** — classifying satellite image patches into land use/land cover categories (EuroSAT dataset)
2. **SAR-to-Optical Image Translation** — translating Synthetic Aperture Radar (SAR) images into optical-like RGB images using a GAN

---

## 1. Land Cover Classification

### Overview
Classifies Sentinel-2 satellite image patches into land cover classes (e.g. residential, industrial, forest, river, crop, pasture, highway) using a convolutional neural network trained from scratch.

### Dataset
- **EuroSAT dataset** — Sentinel-2 satellite images across 10 land cover classes
- *(Add: number of images used, train/val/test split, image resolution)*

### Approach
- **Model:** Custom CNN trained from scratch (no pretrained weights)
- *(Add: number of conv layers, input image size, loss function, optimizer, number of epochs)*

### Results
*(Add accuracy, confusion matrix, or sample predictions)*

| Metric | Value |
|--------|-------|
| Accuracy | TBD |
| F1 Score | TBD |

---

## 2. SAR-to-Optical Image Translation

### Overview
Translates SAR (radar) satellite images — which are hard to interpret visually but work in all weather/lighting conditions — into optical-style RGB images that are easier to interpret, using a Generative Adversarial Network.

### Dataset
*(Add: dataset name/source, e.g. SEN1-2, number of paired SAR/optical image samples)*

### Approach
- **Model:** GAN-based image-to-image translation (e.g. pix2pix/CycleGAN style architecture)
- **Generator:** *(e.g. U-Net based encoder-decoder)*
- **Discriminator:** *(e.g. PatchGAN)*
- *(Add: loss functions used — adversarial loss + L1/L2 loss, number of epochs)*

### Results
*(Add sample outputs: SAR input → generated optical image → ground truth comparison, plus any quantitative metrics like SSIM/PSNR)*

---

## Tech Stack

- Python
- Jupyter Notebook / Google Colab
- *(Add: TensorFlow/Keras or PyTorch, plus any other libraries — NumPy, Matplotlib, rasterio, etc.)*

## Project Structure

```
EUTO-SAT---land-cover-classification-/
├── EUTO_SAT_land_cover_classification_.ipynb   # Land cover classification (CNN)
├── SAR_to_optical_image_translation_.ipynb     # SAR-to-optical translation (GAN)
└── README.md
```

## How to Run

1. Clone the repo
   ```bash
   git clone https://github.com/Mahimajha07/EUTO-SAT---land-cover-classification-.git
   ```
2. Open either notebook in Jupyter or Google Colab
3. Run cells in order (data loading → preprocessing → model → training → evaluation)

## Future Improvements

- Try pretrained backbones (ResNet/EfficientNet) for land cover classification to compare against the from-scratch CNN
- Explore CycleGAN for unpaired SAR-optical translation if paired data is limited
- Combine both pipelines: classify land cover directly on GAN-translated optical images

## Author

**Mahima Jha** — First-year undergraduate, AI & Cyber Security, IIT Patna
[LinkedIn](https://linkedin.com/in/mahima-jha07)
