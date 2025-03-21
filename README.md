# CS5720 - Home Assignment 3

## Overview
This repository contains the solutions for **CS5720 - Home Assignment 3**, covering multiple tasks related to **Autoencoders, RNNs, and Sentiment Classification** using **TensorFlow**. Each task is organized into its own directory with **Jupyter Notebooks (`.ipynb`)**, **Python scripts (`.py`)**, and **README.md** files.

## Repository Structure
```
CS5720-HomeAssignment1/
│── Q1_Autoencoder/
│   ├── HA1_1.ipynb
│   ├── ha1_autoencoder.py
│   ├── README.md
│
│── Q2_Denoising_Autoencoder/
│   ├── HA2_1.ipynb
│   ├── ha2_denoising_autoencoder.py
│   ├── README.md
│
│── Q3_RNN_Text_Generation/
│   ├── HA3_1.ipynb
│   ├── ha3_rnn_textgen.py
│   ├── README.md
│
│── Q4_Sentiment_Classification/
│   ├── HA4_1.ipynb
│   ├── ha4_sentiment_lstm.py
│   ├── README.md
│
├── README.md  # Main ReadMe file
```

## Assignment Breakdown

### **1. Basic Autoencoder** (Q1_Autoencoder)
- Implements a fully connected autoencoder on MNIST.
- Demonstrates reconstruction with different latent dimensions (16, 32, 64).

### **2. Denoising Autoencoder** (Q2_Denoising_Autoencoder)
- Adds Gaussian noise to MNIST images.
- Trains the autoencoder to reconstruct clean images from noisy ones.

### **3. RNN for Text Generation** (Q3_RNN_Text_Generation)
- Builds an LSTM model trained on Shakespeare’s text.
- Generates character-level text using temperature scaling.

### **4. Sentiment Classification** (Q4_Sentiment_Classification)
- Trains an LSTM model on IMDB reviews to classify sentiment.
- Includes confusion matrix and classification report.

## Installation & Requirements
Install the required dependencies:
```sh
pip install tensorflow matplotlib numpy scikit-learn seaborn
```
On **Google Colab**, all dependencies are pre-installed.

## Running the Code
Navigate to the relevant folder and run:
```sh
python HAX_1.ipynb  # Replace X with the corresponding file (e.g., HA1_1.ipynb)
```

## Output Highlights
- Autoencoders visualize reconstructed images (clean vs noisy)
- RNN generates Shakespeare-like text
- Sentiment classifier reports accuracy, precision, recall, and F1-score

## Contact
**Name:** Harshith Reddy Gundra  
**Student ID:** 700780724  
**Email:** hxg07240@ucmo.edu  

---

