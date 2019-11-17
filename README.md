# NLP-2019
You can view all the assignment of the CS 613-NLP here.
The folder contains the following:
* Assignment 1 - Using the "Tweets Dataset" to calculate Token, Types and TTR. Also plotted the Zipf's Law and Heap's Law for the given corpus.
* Assignment 2- Language Modeling ( N-gram and LSTM Approach )
* Assignment 3- Sentiment Analysis on Bi-Lingual Tweets
<br />
Assignment-3  <br />
Submitted by : Prakash R <br />
Roll number : 17110109 <br />

## Pre-Processing:
We removed all the hashtags, links and mentions using regex library in python.
## Embedding:
Embedding was taken for each word from FLARE library and then concatenated to form a embedding vector. Since the size of the sentence are not the same. We used padding.
## Model:
Layer 1: Bidirectional Layer with 128 elements.
Layer 2: 
Layer 3:
## Overall Accuracy:

accuracy = 0.53 <br />
f1_score = 0.53 <br />
precision = 0.54 <br />
recall = 0.55 <br />
            
Model: "sequential" <br />
Layer (type)            <br />  
bidirectional (Bidirectional) <br />
dropout (Dropout)           <br />       
gru (GRU)                   <br />    
dropout_1 (Dropout)        <br />        
dense (Dense)               <br />
