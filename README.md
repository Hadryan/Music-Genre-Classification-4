# Music-Genre-Classification

The full project is available as a pdf:
https://github.com/RMCox/Music-Genre-Classification/blob/master/Musical_Genre_Classification.pdf

References:
Feature extraction with Librosa used base code in the below article
https://towardsdatascience.com/music-genre-classification-with-python-c714d032f0d8

Created and compared 2 Neural Networks to classify a database of 1000 audio tracks into their 10 musical genres: A convolutional neural network trained on visual representations of the audio, and a linear neural network based on extracted musical featues.

* Pre-processed the audio files using functions to pad and crop.
* Extracted key features of the Audio using the Librosa package, e.g. spectral bandwidth.
* Outlier detection to reveal and remove corrupted files.
* for interest, compared musical genres using cosine similarity, created a function to identify similar songs (resulted in tracks by the same artist).

**Convolutional Neural Network**
* Converted audio files to Mel-Spectograms for visual representation.
* Trained a Convolutional Neural Network using Pytorch using ReLU activation functions and dropout.
* Use of model to predict individual tracks, outputting probabilty of each genre.


**Linear Neural Network**
* Used extracted key features to predict labels after addressing multi-colinearity.
* Achieved higher accuracy using extracted features than the visual representation.
* Use of model to predict individual tracks, outputting probabilty of each genre.
