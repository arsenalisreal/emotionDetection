# Emotion Detection Application

Final project for the Coursera course **Developing AI Applications with Python and Flask** (IBM AI Application Developer).

## Project name

**Emotion Detection using Watson NLP**

## Description

This application analyzes text and detects emotions using the IBM Watson NLP Emotion Predict service. It identifies five emotions — anger, disgust, fear, joy, and sadness — and returns the dominant emotion. The application is packaged as `EmotionDetection` and deployed as a Flask web app.

## Features

- Emotion analysis via Watson NLP Emotion Predict API
- Packaged Python module (`EmotionDetection`)
- Unit tests for dominant emotion detection
- Flask web interface at `/emotionDetector`
- Error handling for blank or invalid input
- Static code analysis with pylint

## Project structure

```text
EmotionDetection/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── screenshots/
├── server.py
├── test_emotion_detection.py
└── README.md
```

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install requests flask pylint
```

## Usage

### Python module

```python
from EmotionDetection.emotion_detection import emotion_detector
print(emotion_detector("I love this new technology."))
```

### Unit tests

```bash
python3 test_emotion_detection.py
```

### Flask web app

```bash
python3 server.py
```

Open `http://localhost:5000` in a browser.

### Static code analysis

```bash
pylint server.py
```

## Author

Layla Kamal
