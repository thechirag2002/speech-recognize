# speech-recognize
> USING NLP-Natural Language Processing
A Python script for Recognizing Speech from a ".wav" audio file

## Wav2Vec2-Base-960h 

### [Facebook's Wav2Vec2](https://ai.facebook.com/blog/wav2vec-20-learning-the-structure-of-speech-from-raw-audio/)

> The model facebook wav2vec2 base 960h is a Natural Language Processing (NLP) Model implemented in Transformer library, generally using the Python programming language.


### Whole Process

- Initially, important needed libraries are imported like 

```
torch
librosa
numpy
soundfile
scipy.io.wavfile
IPython.display.Audio 
```

## transformer

A transformer is a deep learning model that adopts the mechanism of self-attention, differentially weighting the significance of each part of the input data.


### Wav2Vec2ForCTC & Wav2Vec2Tokenizer
```
from transformer import Wav2Vec2ForCTC
```
Wav2Vec2ForCTC is used to instantiate a Wav2Vec2 model according to the specified arguments, defining the model architecture.

```
from transformer import Wav2Vec2Tokenizer
```
Wav2Vec2 is a speech model that accepts a float array corresponding to the raw waveform of the speech signal. Wav2Vec2 model was trained using connectionist temporal classification (CTC) so the model output has to be decoded using Wav2Vec2CTCTokenizer.



- **The foundational model was pretrained and fine-tuned using 960 hours of 16kHz sampled speech audio from Librispeech. Make sure your speech input is captured at 16 KHz when utilising the model**

![model](https://github.com/thechirag2002/speech-recognize/blob/24b56ae3f124594563d00e54e96cb4b0b932c805/Wav2Vec2.png)

```OUTPUT for given file```
![output](https://github.com/thechirag2002/speech-recognize/blob/24b56ae3f124594563d00e54e96cb4b0b932c805/output.png)
