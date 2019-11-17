# NLP-2019
You can view all the assignment of the CS 613-NLP here.
The folder contains the following:
* Assignment 1 - Using the "Tweets Dataset" to calculate Token, Types and TTR. Also plotted the Zipf's Law and Heap's Law for the given corpus.
* Assignment 2- Language Modeling ( N-gram and LSTM Approach )
* Assignment 3- Sentiment Analysis on Bi-Lingual Tweets

Assignment-3 
Submitted by : Prakash R
Roll number : 17110109 

## Pre-Processing:
We removed all the hashtags, links and mentions using regex library in python.
## Embedding:
Embedding was taken for each word from FLARE library and then concatenated to form a embedding vector. Since the size of the sentence are not the same. We used padding.
## Model:
0.52969503, 0.51582956, 0.54311556, 0.49189213
accuracy, f1_score, precision, recall

Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
bidirectional (Bidirectional multiple                  3277824   
_________________________________________________________________
dropout (Dropout)            multiple                  0         
_________________________________________________________________
gru (GRU)                    multiple                  16680     
_________________________________________________________________
dropout_1 (Dropout)          multiple                  0         
_________________________________________________________________
dense (Dense)                multiple                  63        
=================================================================
Total params: 3,294,567
Trainable params: 3,294,567
Non-trainable params: 0
________________________________________
