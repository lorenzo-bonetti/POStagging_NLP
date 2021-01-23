# SUMMARY

## Data Preprocessing
Splitted the dataset in train, validation and test sets

Built 3 different vocabularies (one for each set)

Used a co-occurrence matrix to handle OOV words (looking at closest words in the co-occurrence 
 and using the mean of their vectors as embedding for the OOVs)

Built the embedding matrix with GloVe (dim: 300)

Transformed POS tags from strings to categorical encoding

## Training
5 different models have been trained

* Bidirectional LSTM (single layer)
* Bidirectional GRU (single layer)
* Bidirectional LSTM (double layer)
* Bidirectional LSTM (single layer) + CRF
* Bidirectional LSTM (double layer) + CRF

## Evaluation
Accuracy and F1 scores have been evaluated both on training and validation set

F1 scores have been calculated with and without considering punctuation

The model with the best F1-macro (BiCRF) have been evaluated on the test set

## Error analysis
A few considerations on the results obtained are at the end of the notebook

## Credits
Lorenzo Bonetti

Giulio Fortini
