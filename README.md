# Vocally – Speech Emotion Recognition System

A web application that detects emotions from speech. Users upload or record audio, and a fine-tuned Wav2Vec 2.0 model predicts one of 7 emotions.

**Live demo:** https://indru7805.github.io/Speech-Emotion-Recognition-System/ 

## Features
- Classifies speech into 7 emotions: Happy, Sad, Angry, Neutral, Fear, Disgust, Surprise
- Real-time predictions through a Flask web interface
- Full pipeline: audio preprocessing, feature extraction, classification
- [Face emotion page: confirm it works, or delete this line]

## Results
| Metric | Score |
|---|---|
| Accuracy | 80.9% |
| F1-score | 80.9% |

Dataset: 5,000 samples, 7 emotion classes ([dataset name], [train/test split]).

## Tech Stack
- Python, PyTorch, Hugging Face Transformers (Wav2Vec 2.0), Librosa
- Flask, HTML, CSS, JavaScript

## How It Works
1. Audio is loaded and resampled with Librosa.
2. The Wav2Vec 2.0 model, fine-tuned on the dataset, extracts features and classifies the emotion.
3. The Flask app returns the predicted emotion to the page.

## Use Cases
- Customer support: flag frustrated callers
- Mental health: track emotional changes in speech over time
- Interview practice: feedback on tone and confidence

## Getting Started
1. `git clone https://github.com/indru7805/Speech-Emotion-Recognition-System.git`
2. `pip install -r requirements.txt`
3. `python app.py` 
4. Open `http://localhost:5000`

## Project Structure
[run `tree` and paste it]

## Limitations
- Accuracy depends on audio quality and the training data's accents and recording conditions.
- Predictions are probabilistic and shouldn't be used for clinical or hiring decisions.

## Author
Indrajeet Patil – github.com/indru7805
