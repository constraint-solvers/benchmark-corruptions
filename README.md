# benchmark-corruptions
Public repo containing supplementary material for the work submitted to EMNLP-19

This repository hosts the corrupted test sets that were generated to benchmark the robustness of the FastText and Bi-LSTM models as described in the paper
Benchmarking Popular Classification Models' Robustness to Random and Targeted Corruptions
These test sets were derived by applying the two corrupted strategies and the different corruption methods to the test sets of the following datasets:
SST2, IMDB, YELP and DBPEDIA
The repository consists of two folders each corresponding to the respective models used.
The filenames follow the convention:
[DATASET]_[CORRUPTION STRATEGY][CORRUPTION METHOD]_[MODEL]_n
DATASET is the base dataset that was used
CORRUPTION STRATEGY One of Random or LIME based corruption
CORRUPTION METHOD Corresponds to how the selected word was modified (Deleted, Spelling Error Introduced, Text Noise introduced, Replaced by Synonym)
MODEL The model used for LIME explanations
n The number of words changed as per the strategy
PS:
For the fasttext model, the files are in the format LABEL[TAB]TEXT
For the Bi-LSTM model, we use a self-explanatory JSON format to be compatible with AllenNLP
