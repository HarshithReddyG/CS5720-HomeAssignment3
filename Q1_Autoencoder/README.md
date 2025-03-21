# Autoencoder with MNIST

## Overview
This project demonstrates the implementation of a simple **fully connected autoencoder** using **TensorFlow** to reconstruct MNIST digit images. The goal is to understand how dimensionality reduction affects reconstruction quality.

## Dataset
MNIST dataset from `tensorflow.keras.datasets` is used.
- 60,000 training images
- 10,000 test images
- Each image is 28x28 pixels (flattened to 784 for the model)

## Code Flow
1. **Load and Preprocess Data:**
   - Normalize image pixel values to range [0,1].
   - Reshape from (28,28) to (784,) vectors.
2. **Autoencoder Architecture:**
   - **Encoder:** Input (784) → Dense (latent_dim).
   - **Decoder:** Dense (784) with sigmoid activation.
3. **Training Setup:**
   - Use `binary_crossentropy` as loss function.
   - Optimizer: Adam.
   - Trained for 10 epochs with batch size 256.
4. **Evaluation:**
   - Compare original and reconstructed images.
   - Analyze results for latent dimensions: **16**, **32**, **64**.

## Installation & Requirements
### Google Colab:
- TensorFlow pre-installed

### Local:
```sh
pip install tensorflow matplotlib
```

## Running the Script
To run the Python file locally:
```sh
python ha1_autoencoder.py
```

Or open the Colab notebook:
📍 `Q1_Autoencoder/HA1_1.ipynb`

## Output
- Displays plots comparing **original vs reconstructed images** for different latent sizes.
- Visualizes how compression impacts image quality.

## Observations
1. **Latent Dimension 16:**
   - Blurry reconstructions, lower detail retention.
2. **Latent Dimension 32:**
   - Balanced quality and compression.
3. **Latent Dimension 64:**
   - High-quality reconstructions, minimal loss.

## Remarks
- Code is modular and well-commented.
- Only essential logic included.
- Run the Jupyter notebook in `Q1_Autoencoder/HA1_1.ipynb` to visualize outputs interactively.

## Contact
**Name:** Harshith Reddy Gundra  
**Student ID:** 700780724  
**Email:** hxg07240@ucmo.edu  

📍 **Code Path:** `Q1_Autoencoder/HA1_1.ipynb`

