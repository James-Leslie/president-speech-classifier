# Data Science for Industry Project 2: Predict the President
There were two major sections of this assignment:

  - Train a model capable of predicting the speaker of a given sentence taken from a South African presidential address.  
  - Use text mining and sentiment analysis to extract any insights from the text data for all State of the Nation Addresses between 1994 and 2018.   

The data used for this assignment consisted of a collection of text files containing every South African State of the Nation Address given between 1994 and 2018.

## Folder structure
### `data`
  - `speeches`: contains raw `.txt` files, one per speech
  - `0.1_data_loader.ipynb`: loads these speeches into a single file named `speeches.csv`.

### `language-model`
  - `1.1_pre-processing.ipynb`: reads in `speeches.csv`, cleans and processes data and prepares a new file `model_input.csv` for training of the language classifier.
  - `1.2_text_classifier.ipynb`: reads in `model_input`, deals with class imbalance and trains and tests neural network model for classifying sentences.
  - `README.md`: contains further instructions on these notebooks

### `text-mining`
  - `sentiment.Rmd`: reads in `speeches.csv` and performs a sentiment analysis on the text.
  - `text_analytics.Rmd`:reads in raw text-files from the `speeches` folder and performs various text analytics text techniques.
  -`word_cloud.ipynb`: reads in cleaned `model_input.csv` and generates a word cloud of the top 20 most spoken words for each president.
  - `README.md`:contains further instructions on how to run the above files and more information on them.

## Group Participation
This group consisted of Dean Hope Robertson, James Leslie, Kieran Donnelly and Devon Stone.

The language model, class balancing and classifier model sections were handled by James and Kieran. Dean completed the sentiment analysis of the speeches. Devon completed the other text analytics and the word cloud generation. In addition, James wrote the pre-processing and data-loader notebooks and they were annotated by Kieran.

Every group member added to their respective `README.md` files, while this `README.md` was created by Devon. Each group member contributed to the report by writing about the section/s that they completed.

There was a constant screening of communication between group member throughout this project via either Whatsapp or Slack.

We made use of a central Github repo initially, and in order to run the `classifier` notebook on a GPU we moved the repo across to Google Drive, from which we opened notebooks within Google's Colaboratory (or Colab). Colab provides free GPU compute which was incredibly useful in training the neural net quickly and freely.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzY2Nzc2MDAzLDI5OTk0NDYyMV19
-->
