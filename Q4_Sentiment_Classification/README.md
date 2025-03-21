# Sentiment Classification Using LSTM (IMDB Dataset)

## Overview
This project implements a **sentiment classifier** using an **LSTM-based RNN** to classify IMDB movie reviews as **positive or negative**. The model is trained on tokenized and padded sequences from the IMDB dataset.

## Dataset
The IMDB dataset is loaded from `tensorflow.keras.datasets.imdb`:
- 25,000 reviews for training, 25,000 for testing
- Each review is encoded as a sequence of integers
- Top 10,000 most frequent words are used

## Code Flow
1. **Load and Preprocess Data:**
   - Load the dataset with only the top 10,000 words
   - Pad sequences to a uniform length of 200
2. **Model Architecture:**
   - Embedding layer (128 dimensions)
   - LSTM layer (64 units)
   - Dense layer with sigmoid activation for binary classification
3. **Training Setup:**
   - Loss: Binary crossentropy
   - Optimizer: Adam
   - Trained for 3 epochs with batch size of 64
4. **Evaluation:**
   - Confusion matrix and classification report
   - Metrics: Accuracy, Precision, Recall, F1-Score

## Installation & Requirements
### Google Colab:
- No installation required

### Local:
```sh
pip install tensorflow scikit-learn matplotlib seaborn
```

## Running the Script
```sh
python ha4_sentiment_lstm.py
```

📍 Or open: `Q4_Sentiment_Classification/HA4_1.ipynb`

## Output
- Classification report showing precision, recall, F1-score
- Confusion matrix heatmap

## Observations
- LSTM successfully learns review sentiment with good accuracy
- Misclassifications often occur with ambiguous or neutral reviews

## Why Precision-Recall Tradeoff Matters
In sentiment classification:
- **Precision** helps minimize false positives (e.g., predicting a bad review as good)
- **Recall** ensures negative reviews are caught
- **F1-score** balances both — useful when false positives/negatives have real impact (e.g., product reviews, spam detection)

## Real-World Use Case
💬 **Customer Feedback Analysis:**
Businesses use LSTM models to monitor sentiment in user reviews and social media to improve services and marketing.

## Remarks
- Code is minimal and clearly commented
- All evaluation metrics are computed and visualized

## Contact
**Name:** Harshith Reddy Gundra  
**Student ID:** 700780724  
**Email:** hxg07240@ucmo.edu  

📍 **Code Path:** `Q4_Sentiment_Classification/HA4_1.ipynb`

