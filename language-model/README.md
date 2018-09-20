# Language Model
This folder contains the necessary notebooks for training a speech classification model.
  - `pre-processing.ipynb` contains all necessary data cleaning and processing steps.
  - `text-classifier.ipynb` contains workflow for upsampling data, tokenizing words, training and validating a neural network speech classifier.

## 1. Pre-processing
The data contained in `data/speeches.csv` is not ready to be used as input. The following issues first need to be resolved before the data may be used for training a model:
  1. Some lines in the data contain multiple sentences - split these lines on full-stops, question marks, and exclamation marks.
  2. Punctuation and capital letters - need to remove punctuation and convert all letters to lowercase.   

The clean data is then saved into a separate file found in `data/model_input.csv`.

## 2. Classifying sentences
If you do not have a machine with a GPU, Cuda, Tensorflow and Keras installed, this notebook can be run using Google Colab. Head to [https://colab.research.google.com/](https://colab.research.google.com/), where you can load the notebook directly from this GitHub repository.   

Once the notebook is loaded, make sure to enable a GPU-enabled runtime environment:   
`Runtime -> Change runtime type -> Hardware accelerator -> GPU`   

The notebook has been set up to run top-to-bottom, without the need to change any file paths.   

There are two main components of this notebook:
  1. Handling the class imbalance in the data set.
  2. Training and testing a CNN LSTM neural network model on the data set.

### 2.1. Class imbalance
The data set used for this project is heavily imbalanced. A distribution of the number of sentences per president is shown below.   

| President | Sentence Count |
|---|---|
| FW de Klerk | 105 |
| Nelson Mandela |  |
| Thabo Mbeki |   |
| Kgalema Mothlanthe |   |
| Jacob Zuma |   |
| Cyril Ramaphosa |   |
