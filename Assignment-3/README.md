Assignment-3  <br />
Submitted by : Prakash R <br />
Roll number : 17110109 <br />

## Pre-Processing:
We removed all the hashtags, links and mentions using regex library in python.
## Embedding:
Embedding was taken for each word from FLARE library and then concatenated to form a embedding vector. Since the size of the sentence are not the same. We used padding. We used sentence embedding first and the accuracy was around 49% which is less than the word embedding accuracy. The size of the embedding vector is 3072. Which then was passed into the model.
## Model:
Layer 1: An embedding layer of a vector size of 3072. <br />
Layer 2: 128 cell bi-directional LSTM layers, where the embedding data is fed to the network. A dropout of 0.2 is added to prevent overfitting. <br />
Layer 3: A 20 layer GRU layer which takes in the input from the LSTM layer. A Dropout of 0.2 is added here. <br />
Layer 4: A 3 layer dense network at the output with softmax activation, each class is used to represent a sentiment category. 
## Overall Accuracy:

### Accuracy = 0.53 
### F1_score = 0.53 
### Precision = 0.54 
### Recall = 0.55 

## Class-Wise Results
![Results](https://raw.githubusercontent.com/delta-ng/NLP-2019/master/Assignment-3/Results.png)
