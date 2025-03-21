# RNN for Character-Level Text Generation

## Overview
This project implements an LSTM-based **Recurrent Neural Network (RNN)** using **TensorFlow** to generate text at the character level. It learns from Shakespeare's text and generates new sequences based on a seed input.

## Dataset
The **Shakespeare dataset** is automatically downloaded using TensorFlow:
- Input text is tokenized into characters
- Each character is mapped to a unique index
- Sequences of 100 characters are used for training

## Code Flow
1. **Text Preprocessing:**
   - Create character-to-index and index-to-character mappings
   - Convert entire text to integer indices
2. **Model Architecture:**
   - Embedding layer (256 dimensions)
   - LSTM layer (512 units)
   - Dense output layer with vocabulary size
3. **Training Setup:**
   - Batch size: 64, Epochs: 5
   - Optimizer: Adam, Loss: SparseCategoricalCrossentropy
4. **Text Generation:**
   - Generates characters one at a time using the trained model
   - Uses **temperature scaling** to control randomness

## Installation & Requirements
### Google Colab:
- No installation needed

### Local Setup:
```sh
pip install tensorflow
```

## Running the Script
```sh
python ha3_rnn_textgen.py
```

📍 Or open the Colab notebook:  
`Q3_RNN_Text_Generation/HA3_1.ipynb`

## Output
- The model generates character-level text
- Output varies based on the **temperature** value

## Observations
- **Low temperature (e.g. 0.2):** Generates more predictable, repetitive text
- **High temperature (e.g. 1.0):** More creative but also more random and sometimes incoherent

## What is Temperature Scaling?
Temperature controls the randomness of predictions during generation:
- **Low (<1.0):** Sharpens the probability distribution → safer, more repetitive output
- **High (>1.0):** Flattens distribution → more surprising and diverse outputs

## Real-World Use Case
🧠 **Creative Writing Tools:**  
RNNs with temperature scaling are used in AI writing assistants for generating poetry, story plots, and dialogue options.

## Remarks
- Code is self-contained and well-commented
- Easy to run and customize the generation

## Contact
**Name:** Harshith Reddy Gundra  
**Student ID:** 700780724  
**Email:** hxg07240@ucmo.edu  

📍 **Code Path:** `Q3_RNN_Text_Generation/HA3_1.ipynb`

