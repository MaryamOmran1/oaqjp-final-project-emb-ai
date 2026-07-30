# Emotion Detection Project using Watson NLP

## Overview

This project is an AI-based web application built as the final project for IBM Skills Network's **"AI-Based Web Application Development and Deployment"** course.

**Scenario:** You have been hired as a software engineer by an e-commerce company to build an app that analyzes customer feedback on their products and automatically detects the emotions expressed in the text.

Emotion Detection extends the concept of Sentiment Analysis. Instead of simply classifying text as positive or negative, it extracts finer-grained emotions such as:

- Joy
- Sadness
- Anger
- Disgust
- Fear

The system then identifies the **Dominant Emotion** among these.

## Features

- Analyzes user-input text and returns a score for each emotion.
- Identifies the dominant emotion in the text.
- Simple web interface for interacting with the system.
- Error handling (e.g., for blank/empty text input).
- Unit tests to verify the emotion detection function works correctly.

## Project Structure

```
oaqjp-final-project-emb-ai/
├── EmotionDetection/          # Core package containing the emotion detection logic
│   └── emotion_detection.py
├── static/                    # CSS/JS files for the front end
├── templates/                 # HTML files for the web interface
├── server.py                  # Flask server that runs the application
├── test_emotion_detection.py  # Unit tests
├── requirements.txt           # Python dependencies
└── README.md
```

## Technologies Used

- **Python 3**
- **Flask** – for building the web server
- **Watson NLP Embeddable AI Library** – for text analysis and emotion detection
- **HTML/CSS/JavaScript** – for the front end

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/MaryamOmran1/oaqjp-final-project-emb-ai.git
   cd oaqjp-final-project-emb-ai
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the server:
   ```bash
   python server.py
   ```

4. Open your browser and go to:
   ```
   http://localhost:5000
   ```

## Usage

- Open the app in your browser.
- Enter the customer's feedback/comment text in the input field.
- Click the analyze button. The system will return scores for each emotion (Joy, Anger, Disgust, Sadness, Fear) along with the Dominant Emotion.

## Running Tests

```bash
python -m unittest test_emotion_detection.py
```

## License

This project is licensed under the terms in the LICENSE file included in this repository.

## Credits

This project is based on the original IBM Developer Skills Network project:
[ibm-developer-skills-network/oaqjp-final-project-emb-ai](https://github.com/ibm-developer-skills-network/oaqjp-final-project-emb-ai)
