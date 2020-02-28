# Sentence-level Translation Quality Estimation Shared Task 2020

The aim of the task is to develop a a variety of regression models to predict the quality and accuracy of a machine translated sentence given a pair of source (English) and machine translated (German) sentences. To train the models, several pre-processing techniques were applied on the raw dataset of 8000 sentence pairs and multiple methods of embedding the sentence pairs to vector were also constructed to prepare them as input to the models. The embedding methods are then combined with different regressions models to form a model that can predict the quality of a machine translated sentence. Each model is analysed based on the results from the test and challenges such as a biased training dataset are discussed in the paper to provide an insight into the test results.

This repository consists of the following models (and can be found in the respective files):
1. Multilingual BERT with XGBoost (BERT Word-Embeddings.ipynb)
2. BERT (with Named Entity kept) with RFR (BERT Word-Embeddings.ipynb)
3. Keras Tokenization with MLP (Keras Tokenizer.ipynb)
4. BERT (with Named Entity removed and POS tagged) with Rbf SVM (BERT Word-Embeddings.ipynb)
5. BERT (with  Named  Entity removed) with Linear SVM (BERT Word-Embeddings.ipynb)
6. Bag-of-Words with Linear SVM (BoW_SVM.ipynb)


## Results of Model
| Model                                                        | Pearson Coefficient |
| -------------                                                |:-------:| 
| Multilingual BERT with XGBoost                               | 0.1171  |
| BERT (with Named Entity kept) with RFR                       | 0.0847  |   
| Keras Tokenization with MLP                                  | 0.0554  |
| BERT (with Named Entity removed and POS tagged) with Rbf SVM | 0.0279  |
| BERT (with  Named  Entity removed) with Linear SVM           | 0.01096 |
| Bag-of-Words with Linear SVM                                 | -0.0096 |
