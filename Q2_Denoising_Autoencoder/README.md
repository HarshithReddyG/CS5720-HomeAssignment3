# Denoising Autoencoder with MNIST

## Overview
This project implements a **denoising autoencoder** using **TensorFlow** to remove Gaussian noise from MNIST digit images. The model learns to reconstruct clean images from noisy inputs.

## Dataset
MNIST dataset from `tensorflow.keras.datasets` is used:
- 60,000 training images, 10,000 test images
- Images are 28x28 pixels, flattened to vectors of size 784

## Code Flow
1. **Load and Preprocess Data:**
   - Normalize pixel values to [0,1]
   - Flatten images
2. **Add Gaussian Noise:**
   - Add noise with mean=0 and std=0.5 to both train and test sets
   - Clip values to [0,1]
3. **Denoising Autoencoder Architecture:**
   - **Encoder:** Input (784) → Dense(32)
   - **Decoder:** Dense(784) with sigmoid activation
4. **Training Setup:**
   - Optimizer: Adam
   - Loss: Binary crossentropy
   - Trained on noisy inputs, clean targets for 10 epochs
5. **Evaluation:**
   - Visualize **noisy vs. reconstructed images**

## Installation & Requirements
### Google Colab:
- No setup required

### Local:
```sh
pip install tensorflow matplotlib
```

## Running the Script
To run locally:
```sh
python ha2_denoising_autoencoder.py
```

Or open the notebook:
📍 `Q2_Denoising_Autoencoder/HA2_1.ipynb`

## Output
- Side-by-side plots of **noisy input** vs. **denoised output** images.
- Denoising quality can be visually evaluated.

## Observations
- The model successfully removes Gaussian noise, reconstructing digits clearly.
- Compared to a basic autoencoder, the denoising version is more robust when input data is noisy.

## Real-World Use Case
🩺 **Medical Imaging:**
Denoising autoencoders can improve the quality of MRI or X-ray scans by removing background noise or artifacts, helping doctors interpret results more accurately.

## Remarks
- Code is clearly commented and modular.
- Designed to directly compare noisy and clean reconstructions.

## Contact
**Name:** Harshith Reddy Gundra  
**Student ID:** 700780724  
**Email:** hxg07240@ucmo.edu  

📍 **Code Path:** `Q2_Denoising_Autoencoder/HA2_1.ipynb`

