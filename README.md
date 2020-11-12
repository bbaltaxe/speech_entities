# speech_entities
Returns a list of all entities spoken in a short audio clip 

## setup 

`pip install requirements.txt`

`brew install portaudio`

You'll need to have a google cloud platform account. 

This project uses the _Speech to Text API_ and _Cloud Natural Language API_ you can enable and authorize those on the GCP console after creating a new project.

## input file 
Your input audio file will need to be either .wav or .flac
You will need to know the sample rate of your audio file.

## example usage
example usage: 
`python entities_from_speech.python --path file.wav --sample 44100`

outputs all entities (untagged) to `entities.txt`

outputs transcribed audio to `transcribe.txt`


### Acknowledgements
Big shout out to Google's demo code. This repo is primarily a mashup of the following two example files: 

https://github.com/googleapis/python-language/blob/master/samples/v1/language_entities_text.py

https://github.com/googleapis/python-speech/blob/master/samples/snippets/transcribe.py
