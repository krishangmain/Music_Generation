# LSTM's Album Release: Music Generation with LSTM

## Introduction

Welcome to LSTM's Album Release project! In this project, we aim to generate music using Long Short-Term Memory (LSTM) neural networks. We'll be working with MIDI files of classical piano music, focusing primarily on compositions by Frédéric Chopin.

## Setup

To run this project, you can follow these steps:

1. Mount Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')
```

2. Install dependencies:
```bash
!pip install music21
!apt-get install -y lilypond
```

3. Import Libraries and Load Data:
```python
import numpy as np
import pandas as pd
import os
import music21
from music21 import *
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import LSTM, Dense, Dropout
import tensorflow.keras.backend as K
from tensorflow.keras.optimizers import Adamax
import seaborn as sns
import IPython
```

## Loading Data

We start by loading MIDI files of Chopin's compositions and extracting notes and chords from these files to create a corpus.

## Data Exploration

We explore the corpus, examining the distribution of notes and chords. We also simplify the corpus by removing rare notes.

## Data Preprocessing

In this step, we create a dictionary to map notes to indices, encode the corpus, split it into sequences of equal length, and prepare the data for training.

## Model Building

We build an LSTM model for music generation. The model consists of LSTM layers followed by dense layers.

## Evaluating Models

We evaluate the model's performance by plotting learning curves and generating melodies.

## Usage

You can use this project to generate music melodies using LSTM neural networks. Feel free to experiment with different parameters, model architectures, and datasets to create your own unique music compositions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any part of the README according to your preferences or add more sections as needed!
