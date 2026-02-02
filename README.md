# SRGAN – Super Resolution Using GAN

This project implements a **Super-Resolution Generative Adversarial Network (SRGAN)** using **PyTorch** to enhance low-resolution images into high-resolution outputs.  
It runs on **Google Colab with GPU support** and allows users to upload their own images for super-resolution.

---

## Project Overview

**SRGAN (Super-Resolution GAN)** is a deep learning technique that reconstructs high-resolution images from low-resolution inputs by learning image textures, edges, and fine details.

In this project:
- Users upload an image
- The image is downsampled to simulate low resolution
- A **Generator network** upsamples the image
- Results are displayed and saved to **Google Drive**

---

## Features

- Upload custom images (JPG / PNG)
- Low-resolution image simulation
- GAN-based super resolution (Generator)
- Side-by-side visualization
- Google Drive output storage
- GPU acceleration using Colab

---

##  How It Works

1. User uploads an image
2. Image is resized and normalized
3. Low-resolution image is generated using interpolation
4. Generator network upsamples the image
5. Output image is denormalized
6. Final image is saved to Google Drive

---

##  Project Structure
 Super-Resolution-Using-GAN/
 
-->SRGAN.ipynb

-->srgan_generator.pth

-->SRGAN_Output/

  --> super_resolution_output.png
  
-->README.md

---

##  Output

The notebook displays:
- Original Image
- Low-Resolution Image
- Super-Resolution Image

---

##  Requirements

- Google Colab (GPU enabled recommended)
- Python 3.x
- torch
- torchvision
- PIL
- matplotlib

---

##  How to Run

1. Open `SRGAN.ipynb` in Google Colab
2. Enable GPU  
   `Runtime → Change runtime type → GPU`
3. Mount Google Drive
4. Upload an image
5. Run all cells
6. Output saved in `SRGAN_Output/`

---

## Applications

- 🛰️ Satellite & aerial image enhancement
- 🏥 Medical image super-resolution
- 🔐 CCTV and security footage enhancement
- 🎥 Image and video upscaling
- 🎮 Gaming and AR/VR textures

---

## Future Improvements

- Add Discriminator network
- Train on large datasets (DIV2K, CelebA, Satellite data)
- Add residual blocks
- Use perceptual loss (VGG)
- Batch image processing support

---

## Author

**Swamy Hyma Kumar Vechalapu**  
Deep Learning | Computer Vision | GANs

