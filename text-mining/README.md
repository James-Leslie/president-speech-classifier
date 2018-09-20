# Text Mining

This section of the assignment covered the descriptive analysis of the text in the presidential speeches.

The folder contains the following files:

* ### `text_analytics.Rmd`

This markdown displays the various text analysis techniques used on the text in the speeches. The file first displays how to bring in the raw text-files into R. Then moves onto pre-processing steps such as removing punctuation, stemming words, removing stopwords and how to tokenize the words in the speeches. The markdown then displays how to generate a document term matrix from the speeches.   

After the pre-processing steps the R markdown file documents how to create a count-dictionary to find the major topics of each speech. Then describes how to developed an LDA topic model and finally details how to plot keyness plots.  

The markdown file should be run from top-to-bottom and uses the raw text-files as input.


* ### `word_cloud.ipynb`

This Jupyter notebook generates a word cloud of the twenty most common words spoken by each president in all of their speeches.

The notebook uses the cleaned sentences in the model-input.csv file, which is contained in the data folder. The notebook is run from top to bottom.  


* ### `Sentiment.Rmd`

This markdown displays various sentiment analysis techniques that were performed on the SONA presidential speeches. The data is loaded via URL to the GitHub repository.

The markdown firsts looks at individual word sentiment using popular lexicons as well a overall sentiment of the entire text. The analysis covers sentiment over time using a combination of lexicons, before moving onto n-grams. Finally the markdown looks at how to deal with negators/amplifiers in text as well as calculating polarity scores.

The R markdown file should be run top-to-bottom.
