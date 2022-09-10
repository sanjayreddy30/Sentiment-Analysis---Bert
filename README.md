## Project Overview:
1) Fine-tuned pytorch BERT model with custom final layer to classify the sentiment of message into 5 categories
2) Pre-processed and analysed the data using pandas, split the dataset into training and validation sets in stratified approach
3) Encoded dataset using a pretrained BERT tokenizer and controlled the learning rate of model using AdamW optimizer.
4) Created data loaders to facilitate batch processing, added a training loop to control tuning of BERT using CPU or GPU
5) Evaluated using F1_Score and accuracy rate, achieved a score of 0.86 and 0.79 on validation set respectively
