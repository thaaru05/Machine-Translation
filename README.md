# Machine-Translation

Machine Translation 
This repository contains the implementation of a Multilingual Machine Translation System leveraging state-of-the-art models such as Whisper, mBART, and Text-to-Speech (TTS) pipelines. This project focuses on translating spoken language to another language through three phases: Speech to Text, Text to Text, and Text to Speech.

Table of Contents
Project Overview
Features
Installation
Usage
Project Phases
Technologies Used
Contributing

Project Overview
The goal of this project is to build a multilingual machine translation system that translates speech from one language to another. It integrates Whisper for speech recognition, mBART for multilingual text translation, and TTS (Text-to-Speech) for generating speech output. This system aims to facilitate real-time communication across languages, making it useful for cross-cultural interaction, global customer support, or international collaboration.

Key Objectives:
Translate spoken language to text in the original language.
Translate the text into a target language.
Convert the translated text back to speech in the target language.
Features
Real-Time Speech Translation: Convert speech input to translated speech output with minimal delay.
Support for Multiple Languages: Supports translation between multiple language pairs.
High Accuracy: Uses Whisper for highly accurate speech-to-text, and mBART for multilingual translation.
Modular Architecture: The system is broken down into clear phases to support flexibility and scalability.
OpenAI Whisper Model: Used for high-quality speech recognition.
TTS (Text-to-Speech): Converts translated text to human-like speech using OpenAI TTS.
Installation
Prerequisites
Python 3.7 or higher
GPU (Optional but recommended for faster inference)
Git
Dependencies listed in requirements.txt
Steps
Clone the Repository

bash
Copy code
git clone https://github.com/thaaru05/Machine-Translation.git
cd Machine-Translation
Create a Virtual Environment

bash
Copy code
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
Install Dependencies

bash
Copy code
pip install -r requirements.txt
Set Up API Keys (if applicable)

Ensure you have access to any required API keys for models or cloud services.
Usage
Running the Translation Pipeline
Speech to Text:

Convert spoken language to text using Whisper.
bash
Copy code
python speech_to_text.py --input "path_to_audio_file"
Text to Text Translation:

Translate the text from source language to the target language using mBART.
bash
Copy code
python text_translation.py --source "detected_text" --target_lang "fr"
Text to Speech:

Convert translated text back into speech using TTS.
bash
Copy code
python text_to_speech.py --text "translated_text"
Example
bash
Copy code
python speech_to_text.py --input "sample_audio.wav"
python text_translation.py --source "sample_text" --target_lang "de"
python text_to_speech.py --text "übersetzter Text"
Project Phases
Speech to Text: Using Whisper for highly accurate speech recognition.
Text to Text: Leveraging mBART for translation between languages.
Text to Speech: OpenAI TTS model generates human-like speech in the target language.
Technologies Used
OpenAI Whisper: For Speech-to-Text conversion.
mBART: Multilingual BART for Text-to-Text Translation.
TTS: For Text-to-Speech conversion.
Python: Primary language for scripting.
Hugging Face Transformers: Core library for models.
Contributing
Contributions are welcome! Please follow these steps if you'd like to contribute:

Fork the repository.
Create a new branch (git checkout -b feature-name).
Commit your changes (git commit -m 'Add new feature').
Push to the branch (git push origin feature-name).
Open a pull request.
