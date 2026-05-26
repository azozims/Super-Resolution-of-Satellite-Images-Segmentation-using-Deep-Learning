# 🛰️ Satellite Image Super-Resolution & Segmentation

Deep learning project for **satellite image super-resolution and semantic segmentation** using the **ISPRS Potsdam Dataset**.
The models enhance low-resolution aerial images by 4× while simultaneously classifying each pixel into categories such as buildings, roads, trees, vegetation, and cars.

## 🔍 Features

* 4× image super-resolution
* Pixel-wise semantic segmentation
* Multi-task learning architecture
* Comparison of three deep learning models
* Evaluation using PSNR, SSIM, mIoU, and Pixel Accuracy

## 🧠 Implemented Models

### 1. Convolutional Autoencoder

* Encoder–decoder architecture
* Lightweight and fast training
* Includes segmentation head

### 2. SRResNet

* Residual network with pixel-shuffle upsampling
* ASPP segmentation module
* Best overall performance

### 3. ESPCN

* Efficient sub-pixel convolution network
* Faster and computationally efficient
* Balanced speed and quality

## 📂 Dataset

**ISPRS Potsdam 2D Semantic Labeling Dataset**

* ~2400 RGB aerial image patches
* 6 segmentation classes
* Super-resolution scale: ×4

Classes:

* Roads / Impervious surfaces
* Buildings
* Vegetation
* Trees
* Cars
* Background clutter

## ⚙️ Tech Stack

* Python
* PyTorch
* OpenCV
* Scikit-image
* Matplotlib

## 🚀 Running the Project

Install dependencies:

```bash
pip install torch torchvision opencv-python scikit-image matplotlib tqdm scipy
```

Open and run any notebook:

* `sresnet_potsdam.ipynb`
* `espcn_potsdam_fixed.ipynb`
* `autoencoder_potsdam_fixed.ipynb`

## 📊 Evaluation Metrics

* **PSNR** — Image reconstruction quality
* **SSIM** — Structural similarity
* **mIoU** — Segmentation accuracy
* **Pixel Accuracy** — Correctly classified pixels

## 📁 Project Structure

```bash
├── autoencoder_potsdam_fixed.ipynb
├── sresnet_potsdam.ipynb
├── espcn_potsdam_fixed.ipynb
├── models/
├── samples/
└── patches/
```

## 💾 Pretrained Models

Saved model weights are available inside the `models/` directory for all implemented architectures.
