# Machine-Translation


# Multilingual Machine Translation System

This repository contains the implementation of a **Multilingual Machine Translation System** leveraging state-of-the-art models such as Whisper, mBART, and Text-to-Speech (TTS) pipelines. This project focuses on translating spoken language to another language through three phases: Speech to Text, Text to Text, and Text to Speech.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Phases](#project-phases)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)


## Project Overview

The goal of this project is to build a multilingual machine translation system that translates speech from one language to another. It integrates **Whisper** for speech recognition, **mBART** for multilingual text translation, and **TTS** (Text-to-Speech) for generating speech output. This system aims to facilitate real-time communication across languages, making it useful for cross-cultural interaction, global customer support, or international collaboration.

### Key Objectives:
- Translate spoken language to text in the original language.
- Translate the text into a target language.
- Convert the translated text back to speech in the target language.

## Features

- **Real-Time Speech Translation**: Convert speech input to translated speech output with minimal delay.
- **Support for Multiple Languages**: Supports translation between multiple language pairs.
- **High Accuracy**: Uses Whisper for highly accurate speech-to-text, and mBART for multilingual translation.
- **Modular Architecture**: The system is broken down into clear phases to support flexibility and scalability.
- **OpenAI Whisper Model**: Used for high-quality speech recognition.
- **TTS (Text-to-Speech)**: Converts translated text to human-like speech using OpenAI TTS.

## Installation

### Prerequisites

- Python 3.7 or higher
- GPU (Optional but recommended for faster inference)
- Git
- Dependencies listed in `requirements.txt`

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/thaaru05/Machine-Translation.git
   cd Machine-Translation
   ```

2. **Create a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up API Keys (if applicable)**
   - Ensure you have access to any required API keys for models or cloud services.

## Usage

### Running the Translation Pipeline

1. **Speech to Text**:
   - Convert spoken language to text using Whisper.
   ```bash
   python speech_to_text.py --input "path_to_audio_file"
   ```

2. **Text to Text Translation**:
   - Translate the text from source language to the target language using mBART.
   ```bash
   python text_translation.py --source "detected_text" --target_lang "fr"
   ```

3. **Text to Speech**:
   - Convert translated text back into speech using TTS.
   ```bash
   python text_to_speech.py --text "translated_text"
   ```

### Example
   ```bash
   python speech_to_text.py --input "sample_audio.wav"
   python text_translation.py --source "sample_text" --target_lang "de"
   python text_to_speech.py --text "übersetzter Text"
   ```

## Project Phases

1. **Speech to Text**: Using Whisper for highly accurate speech recognition.
2. **Text to Text**: Leveraging mBART for translation between languages.
3. **Text to Speech**: OpenAI TTS model generates human-like speech in the target language.

## Technologies Used

- **OpenAI Whisper**: For Speech-to-Text conversion.
- **mBART**: Multilingual BART for Text-to-Text Translation.
- **TTS**: For Text-to-Speech conversion.
- **Python**: Primary language for scripting.
- **Hugging Face Transformers**: Core library for models.

## Contributing

Contributions are welcome! Please follow these steps if you'd like to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

