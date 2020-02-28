# Sentence-level Quality Estimation Shared Task 2020

This repository consists of the following models:
1. Multilingual BERT with XGBoost
2. BERT (with Named Entity kept) with RFR
3. Keras Tokenization with MLP
4. BERT (with Named Entity removed and POS tagged) with Rbf SVM
5. BERT (with  Named  Entity removed) with Linear SVM
6. Bag-of-Words with Linear SVM


## Results of Model
| Model                                                        | Pearson |
| -------------                                                |:-------:| 
| Multilingual BERT with XGBoost                               | 0.1171  |
| BERT (with Named Entity kept) with RFR                       | 0.0847  |   
| Keras Tokenization with MLP                                  |         |
| BERT (with Named Entity removed and POS tagged) with Rbf SVM | 0.0279  |
| BERT (with  Named  Entity removed) with Linear SVM           | -0.0057 |
| Bag-of-Words with Linear SVM                                 | -0.0096 |