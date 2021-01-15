# SUMMARY

## Data Preprocessing
-splitted the dataset in train, validation and test sets

-built 3 different vocabularies (one for each set)

-used a co-occurrence matrix to handle OOV words (looking at closest words in the co-occurrence 
 and using the mean of their vectors as embedding for the OOVs)

-built the embedding matrix with GloVe (dim: 300)

-transformed POS tags from strings to categorical encoding

## Training
5 different models have been trained

-Bidirectional LSTM (single layer)

-Bidirectional GRU (single layer)

-Bidirectional LSTM (double layer)

-Bidirectional LSTM (single layer) + CRF

-Bidirectional LSTM (double layer) + CRF

## Evaluation
-accuracy and F1 scores have been evaluated both on training and validation set

-F1 scores have been calculated with and without considering punctuation

-the model with the best F1-macro (BiCRF) have been evaluated on the test set

## Error analysis
A few considerations on the results obtained are at the end of the notebook
