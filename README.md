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
