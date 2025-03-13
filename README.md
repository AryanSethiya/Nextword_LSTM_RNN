# Next Word Prediction using LSTM

This project aims to develop a deep learning model for predicting the next word in a given sequence of words. The model is built using Long Short-Term Memory (LSTM) networks, which are well-suited for sequence prediction tasks.

## Project Overview

The project follows these steps:

### 1. Data Collection
We use the text of Shakespeare's *Hamlet* as our dataset. This rich, complex text provides a good challenge for our model.

### 2. Data Preprocessing
- The text data is tokenized, converted into sequences, and padded to ensure uniform input lengths.
- The sequences are then split into training and testing sets.

### 3. Model Building
- An LSTM model is constructed with:
  - An embedding layer
  - Two LSTM layers
  - A dense output layer with a softmax activation function  
- The softmax activation function predicts the probability of the next word.

### 4. Model Training
- The model is trained using the prepared sequences.
- Early stopping is implemented to prevent overfitting.
- Early stopping monitors the validation loss and stops training when the loss stops improving.

### 5. Model Evaluation
- The model is evaluated using a set of example sentences to test its ability to predict the next word accurately.

### 6. Deployment
- A **Streamlit** web application is developed.
- Users can input a sequence of words and get the predicted next word in real-time.

## 🚀 Live Demo
Try the app here: [Next Word Prediction App](https://nextwordlstmrnn-nkhohunrylhjimh3tlddb5.streamlit.app/)

## Technologies Used
- Python
- TensorFlow/Keras
- Streamlit
- Natural Language Processing (NLP)

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/next-word-prediction.git
   cd next-word-prediction
    ```
2.Create and activate a virtual environment:

```sh
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
.venv\Scripts\activate     # Windows
```

Install dependencies:

```sh
pip install -r requirements.txt
```
Run the Streamlit application:

```sh

streamlit run app.py
```
## Usage
Open the Streamlit web app.
Enter a sequence of words.
Get the predicted next word.

## Contributing
Feel free to fork the project and submit pull requests to improve it.
