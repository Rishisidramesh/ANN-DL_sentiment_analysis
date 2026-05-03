# ANN-DL Sentiment Analysis

This project is a collaborative effort by a team of 4 members to perform **binary sentiment analysis** on movie reviews using **Artificial Neural Networks (ANN)** and **Deep Learning (DL)** techniques.

---

## Project Overview

The goal of this project is to classify movie reviews as **Positive 😊** or **Negative 😞** using a deep learning model trained on the IMDB dataset. The model leverages **LSTM (Long Short-Term Memory)** networks to capture sequential patterns in text data.

---

## Key Features

* Binary sentiment classification (Positive / Negative)
* Uses IMDB Movie Review Dataset (preloaded via TensorFlow/Keras)
* Deep Learning model with:

  * Embedding Layer
  * LSTM Layer
  * Dense Output Layer (Sigmoid)
* Hyperparameter tuning using **Keras Tuner**
* Achieved ~**85.7% test accuracy**
* Real-time sentiment prediction from user input

---

## Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Keras Tuner

---

## Dataset

* IMDB Dataset (50,000 reviews)
* Preprocessed using:

  * Tokenization (Top 10,000 words)
  * Padding sequences to fixed length (200)

---

## Model Architecture

* **Embedding Layer** (learns word representations)
* **LSTM Layer** (captures sequential dependencies)
* **Dense Layer** with Sigmoid activation (binary output)

---

## Hyperparameter Tuning

Used **Random Search** to optimize:

* Embedding dimensions
* LSTM units
* Dropout & recurrent dropout
* Learning rate

### Best Parameters Found:

* Embedding Dimension: 192
* LSTM Units: 32
* Dropout: 0.1
* Recurrent Dropout: 0.1
* Learning Rate: 0.01

---

## Results

* **Validation Accuracy:** ~86.98%
* **Test Accuracy:** ~85.74%
* **Test Loss:** 0.3369

---

## Example Prediction

Input:

```
the matrix
```

Output:

```
Prediction: Positive 😊
Confidence: 65.60%
```

---

## How to Run

1. Install dependencies:

```
pip install tensorflow keras keras-tuner numpy
```

2. Run the script:

```
python main.py
```

3. Enter a movie name or review when prompted.

---

## Team Members

This is a collaborative project developed by a team of 4 members.

---

## Future Improvements

* Use pre-trained embeddings (Word2Vec, GloVe)
* Try Transformer-based models (BERT)
* Improve inference by using full review text instead of movie name
* Deploy as a web app (Streamlit / Flask)

---

## Conclusion

This project demonstrates how deep learning models like LSTM can effectively perform sentiment analysis on textual data. With further optimization and advanced architectures, performance can be significantly improved for real-world applications.

---

⭐ If you like this project, feel free to star the repository!
