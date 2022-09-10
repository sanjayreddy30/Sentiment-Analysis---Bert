## BERT:
Bidirectional Encoder Representations from Transformers (BERT) is a transformer-based machine learning technique for natural language processing (NLP) pre-training developed by Google. BERT was created and published in 2018 by Jacob Devlin and his colleagues from Google. In 2019, Google announced that it had begun leveraging BERT in its search engine, and by late 2020 it was using BERT in almost every English-language query. A 2020 literature survey concluded that "in a little over a year, BERT has become a ubiquitous baseline in NLP experiments", counting over 150 research publications analyzing and improving the model.
BERT is at its core a transformer language model with a variable number of encoder layers and self-attention heads. The architecture is "almost identical" to the original transformer implementation in Vaswani et al.BERT was pretrained on two tasks: language modeling (15% of tokens were masked and BERT was trained to predict them from context) and next sentence prediction (BERT was trained to predict if a chosen next sentence was probable or not given the first sentence). As a result of the training process, BERT learns contextual embeddings for words. After pretraining, which is computationally expensive, BERT can be finetuned with fewer resources on smaller datasets to optimize its performance on specific tasks.

![BERT_diagrams](https://user-images.githubusercontent.com/112507238/189498615-a0e0a4eb-efe7-4181-ae68-d33ccaef9f4d.png)


## How to run
1) Download the files
2) In the second line of .ipynb file, change the path of the smile_annotations.csv file to its current path in the system
3) Insert the name of model (Eg. finetuned_bert_epoch_1_gpu_trained.model) in loading model section to run the model
3) Run all the lines in .ipynb file to get the results
4) To get more accurate results the number of epochs can be increased


## Project Overview:
1) Fine-tuned pytorch BERT model with custom final layer to classify the sentiment of message into 5 categories
2) Pre-processed and analysed the data using pandas, split the dataset into training and validation sets in stratified approach
3) Encoded dataset using a pretrained BERT tokenizer and controlled the learning rate of model using AdamW optimizer.
4) Created data loaders to facilitate batch processing, added a training loop to control tuning of BERT using CPU or GPU
5) Evaluated using F1_Score and accuracy rate, achieved a score of 0.86 and 0.79 on validation set respectively
