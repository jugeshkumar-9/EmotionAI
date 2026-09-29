# EmotionAI: Emotion Prediction from Text

EmotionAI is a deep learning project that detects the emotion in a sentence. It uses a **Bidirectional GRU (BiGRU)** model built with TensorFlow/Keras and provides a **FastAPI** backend for real-time predictions.

## Features
- Predicts 6 emotions: **sadness, joy, love, anger, fear, surprise**
- BiGRU deep learning model trained on the Emotion dataset (Hugging Face)
- Fast REST API built with FastAPI
- Interactive API testing with Swagger UI (`/docs`)
- Simple web interface served as static files

## Tech Stack
- Python
- TensorFlow / Keras
- FastAPI and Uvicorn
- NumPy, Pandas
- Hugging Face `datasets`

## Project Structure
```
EmotionAI/
├── Artifacts/        # Trained model and tokenizer files
├── static/           # Frontend files
├── main.py           # FastAPI application
└── requirements.txt


## How It Works
1. The input text is converted to numbers using a saved tokenizer.
2. The sequence is padded to a fixed length.
3. The BiGRU model predicts the probability of each emotion.
4. The emotion with the highest probability is returned.

## Model Performance
Accuracy: 98%

