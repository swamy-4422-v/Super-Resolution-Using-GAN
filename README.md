SRGAN – Super Resolution Using GAN:

This project implements a Super-Resolution Generative Adversarial Network (SRGAN) using PyTorch to enhance low-resolution images into high-resolution outputs.
It is designed to run on Google Colab with GPU support and allows users to upload their own images for super-resolution.

Project Overview:

SRGAN (Super-Resolution GAN) is a deep learning approach that reconstructs high-resolution images from low-resolution inputs by learning textures, edges, and fine details.

In this implementation:

A user uploads an image.

The image is downsampled to simulate low resolution.

A Generator network upsamples the image.

Outputs are visualized and saved to Google Drive.

✨ Key Features

📤 User Image Upload (JPG / PNG)

🔽 Low-Resolution Simulation

🤖 GAN-Based Super Resolution

🖼️ Side-by-Side Visualization

☁️ Google Drive Integration

⚡ GPU Acceleration (Colab)

🧠 How It Works

Image Upload
User uploads an image via Google Colab.

Preprocessing

Image resized to 128 × 128

Normalized to [-1, 1]

Converted to tensor

Low-Resolution Creation

Downsampled using interpolation (scale_factor = 0.5)

Generator Network

Convolutional layers extract features

Bilinear upsampling increases resolution

Final convolution reconstructs RGB image

Super-Resolution Output

Generator predicts high-resolution image

Output is denormalized and saved

Visualization

Original Image

Low-Resolution Image

Super-Resolution Output

🏗️ Project Structure
SRGAN/
│
├── SRGAN.ipynb                  # Main Google Colab notebook
├── srgan_generator.pth          # Saved Generator model
├── SRGAN_Output/
│   └── super_resolution_output.png
└── README.md

🧩 Generator Architecture

Conv2D (3 → 64)

ReLU

Upsample (scale_factor = 4)

Conv2D (64 → 3)

Tanh

⚠️ Note: This implementation focuses on the Generator only (no Discriminator training).

📊 Output Example
Original Image	Low Resolution	Super Resolution
High quality	Downsampled	GAN enhanced
🛠️ Requirements

Google Colab (GPU enabled recommended)

Python 3.x

PyTorch

torchvision

PIL

matplotlib

▶️ How to Run

Open the notebook in Google Colab

Enable GPU
Runtime → Change runtime type → GPU

Mount Google Drive

Upload an image

Run all cells

View and download results from SRGAN_Output/

🌍 Applications

🛰️ Satellite & Aerial Imaging

🏥 Medical Imaging (MRI / CT)

🔐 CCTV & Security Footage Enhancement

🎥 Video & Photography Upscaling

🎮 Gaming & AR/VR Texture Enhancement

📌 Future Improvements

Add Discriminator Network

Train on large datasets (DIV2K, CelebA, Satellite Images)

Use Residual Blocks

Add Perceptual Loss (VGG)

Support batch image processing

👨‍💻 Author

Swamy Hyma Kumar Vechalapu
📌 Deep Learning | Computer Vision | GANs
