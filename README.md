# Extractive summarization through sentence embedding clustering 

## Introduction

This code sets the basis for a sequential cluster-based algorithm for text summarization. <br>
The summarization technique used in this project is ideally used for highly repetitive text with short answers on specific subjects. <br>
Examples of data on which the algorithm performs well are: <br> 
*  Product/service reviews
*  Open answers to survey questions

## Prerequisites 

The code in this project uses word vectorization with the Word2Vec algorithm and the TF-IDF algorithm. <br> 
To re-run this project you require a pre-trained Word2Vec model, either trained completely on the data at hand or pre-trained and trained partly on the data at hand (transfer learning). <br> 
<br>
The Word2Vec model is read in as _embeddings.bin_. A dictionary should also be provided, with each word in the vocabulary as a key, and its respective vector as a value. In the project, this dictionary was saved as a pickle file and read in as _embedding_dict.pkl_. <br>
The TF-IDF model can be trained on the data at hand and saved as _tfidf.mod_.

## Data source

To run the code, a dataframe is required including the columns for question text (named: QuestionText) and open answers (named: AnswerText). <br> 
An optional third column called SurveyID can be used, when working with data containing multiple surveys.  

## Contribution 

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. <br>

Please make sure to update tests as appropriate.
