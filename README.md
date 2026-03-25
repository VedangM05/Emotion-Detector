# Emotion-Detector

A production-quality Python application using IBM Watson NLP to detect emotions in text.

## Features
- Deep sentiment analysis (Anger, Disgust, Fear, Joy, Sadness)
- Identifies the dominant emotion
- REST API using Flask
- Comprehensive unit tests
- PEP8 compliant code (pylint score 10/10)

## Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/VedangM05/Emotion-Detector.git
   cd Emotion-Detector
   ```

2. Install dependencies:
   ```bash
   pip3 install -r requirements.txt
   ```

## Usage Instructions

### Run the Flask server
```bash
python3 server.py
```

### Accessing the API via Curl
```bash
curl "http://localhost:5000/emotionDetector?textToAnalyze=I%20am%20so%20happy%20today"
```

### Response Example
```
For the given statement, the system response is 'anger': 0.01, 'disgust': 0.01, 'fear': 0.01, 'joy': 0.95, 'sadness': 0.02. The dominant emotion is joy.
```

## Running Unit Tests
```bash
python3 test_emotion_detection.py
```

## Running Static Code Analysis (Pylint)
```bash
pylint server.py
pylint EmotionDetection/emotion_detection.py
```
