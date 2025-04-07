# Speech Recognition & Grammar Scoring System

This project implements a speech-based grammar scoring engine that converts voice input to text and evaluates its grammatical quality using a fine-tuned transformer model.

## Features

- Speech recognition using `SpeechRecognition` and `PyAudio`
- Grammar correction and scoring using a fine-tuned T5 model
- Returns a grammar quality score (scale: 1 to 10)
- Structured as a Jupyter Notebook for ease of use
- Accepts custom-trained models for scoring

## Project Structure

speech_recognition/ ├── Main_code.ipynb # Main code in Jupyter Notebook ├── grammar_dataset/ │ └── Grammar_Correction.csv # Dataset used for model training ├── grammar_model/ # Folder for model files (large model file not included) └── README.md # Project documentation

bash
Copy
Edit

## Getting Started

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Priya-kumari-hub/Grammar_scoring.git
   cd Grammar_scoring
Install the required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Open and run the notebook:

Launch Jupyter Notebook.

Open Main_code.ipynb.

Execute cells sequentially.

Note: The grammar model (model.safetensors) is not included due to GitHub’s 100MB file size limit. You can download or train your own and place it inside the grammar_model/ folder.

Sample Output
Input: what is your name

Corrected: What is your name?

Grammar Score: 9/10

Requirements
Make sure the following Python libraries are installed:

transformers
torch
SpeechRecognition
pyaudio
librosa
pandas
numpy
scikit-learn
