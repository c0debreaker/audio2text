# audio2text
This repo is meant as a guide for generating audio based on speech. This is different from extracting subtitles or more commonly known as closed captions. The `vosk` module requires the input audio file to be in WAV format pcm mono. The output generates a file in json format. It is not perfect but it works.

A model is required. I've included a link to a small model which is about 36 megabytes.

## Requirements
- vosk
- Python no lower than 3.8
- pip

## Installation

1. git clone  https://github.com/c0debreaker/audio2text

2. cd audio2text

3. python3 -m venv venv

4. source venv/bin/activate

5. pip install vosk

6. wget http://alphacephei.com/vosk/models/vosk-model-small-en-us-0.3.zip

7. Extract the zip file to the current folder and rename it to model

8. git clone https://github.com/alphacep/vosk-api

9. python vosk-api/python/example/test_simple.py <your-input.wav> > <any-filename-output.json>