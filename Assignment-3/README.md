Assignment-3  <br />
Submitted by : Prakash R <br />
Roll number : 17110109 <br />

## Pre-Processing:
We removed all the hashtags, links and mentions using regex library in python.
## Embedding:
Embedding was taken for each word from FLARE library and then concatenated to form a embedding vector. Since the size of the sentence are not the same. We used padding.
## Model:
Layer 1: An embedding layer of a vector size of 3072. <br />
Layer 2: 128 cell bi-directional LSTM layers, where the embedding data is fed to the network. A dropout of 0.2 is added to prevent overfitting. <br />
Layer 3: A 20 layer GRU layer which takes in the input from the LSTM layer. A Dropout of 0.2 is added here. <br />
Layer 4: A 3 layer dense network at the output with softmax activation, each class is used to represent a sentiment category. 
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

![Alt text](../master/Assignment-3/Results.png)
