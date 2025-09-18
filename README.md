# Image Colorization with ResNet and GAN

This project focuses on **automatic colorization of grayscale images** using deep learning. The goal is to transform black-and-white flower images into  colored images by learning patterns from the Oxford Flowers102 dataset.

---

## Key Features

* **ResNet18 Encoder:** A modified ResNet18 extracts rich features from grayscale (L channel) flower images. The first layer accepts a single channel and is pretrained on ImageNet for better feature representation.

* **GAN Decoder with PatchGAN Discriminator:** The generator predicts ab color channels, while a PatchGAN-style discriminator evaluates realism via a 7×7 probability map. The model produces vibrant, realistic colorizations.

* **End-to-End LAB Learning:** The network learns directly from L → ab pairs in LAB color space, improving color accuracy and contextual coherence.

* **Visualization:** Outputs are converted back to RGB and displayed **side-by-side** with grayscale input and real color images for easy comparison.

---

## Technologies Used

* Python, PyTorch
* ResNet18 (modified for 1-channel input)
* GANs (Generator + PatchGAN Discriminator)
* Jupyter Notebook for experimentation and visualization

---

## Outcome

The trained model successfully colorizes grayscale flower images from the Oxford Flowers102 dataset, producing visually appealing and contextually accurate results. LAB→RGB conversion and side-by-side visualization demonstrate the model’s effectiveness in realistic color prediction.
