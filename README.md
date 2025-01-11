# POS Tagging for Nepali Dataset  

This repository contains implementations for Part-of-Speech (POS) tagging in Nepali using various machine learning and deep learning models. The project uses the **POS Tagged Nepali Corpus** developed by the **CRULP (Center for Research in Urdu Language Processing)**.  

## Dataset  
The dataset includes 43 tags such as **Noun**, **Verb**, **Adjective**, **Adverb**, and more.  
- Developed by **CRULP**.  
- Derived by translating **100,720 English words** and **4,325 sentences** from the **PENN Treebank**, provided by the **Linguistic Data Consortium (LDC)**.  

## Embedding Techniques
   - **Bare Embedding**: Each word is directly mapped to a randomly initialized vector space.  
   - **Word2Vec Embedding**: Pretrained word embeddings are used to represent words in a dense vector space, capturing semantic relationships.  

## Models Implemented  
This project explores multiple approaches for POS tagging:  
1. **RandomForestClassifier**: A machine learning approach using scikit-learn.  
2. **Vanilla RNN**: A simple Recurrent Neural Network model.  
3. **LSTM (Long Short-Term Memory)**: A neural network designed for sequence modeling.  
4. **GRU (Gated Recurrent Unit)**: A variant of RNN, optimized for long sequences.  
5. **BiLSTM (Bidirectional LSTM)**: An extension of LSTM that looks at both past and future contexts.  
6. **NepBERTa**: A transformer-based model fine-tuned for POS tagging in Nepali.  

## Results  
This project evaluates the performance of various models using different embedding techniques. The table below summarizes the results (fill in the metrics after evaluation):  

| Model            | Embedding         | Accuracy (%) | F1-Score (%) |  
|-------------------|-------------------|--------------|--------------|  
| RandomForest      | N/A               | 77.36        | 76.75        |  
| Vanilla RNN       | Bare Embedding    | 97.65        | 98.00        |  
| Vanilla RNN       | Word2Vec          | 97.90        | 98.00        |  
| LSTM              | Bare Embedding    | 97.21        | 97.00        |  
| LSTM              | Word2Vec          | 97.82        | 98.00        |  
| GRU               | Bare Embedding    | 97.87        | 98.00        |  
| GRU               | Word2Vec          | 98.39        | 98.00        |  
| BiLSTM            | Bare Embedding    | 98.02        | 98.00        |  
| BiLSTM            | Word2Vec          | 98.46        | 98.00        |  
| NepBERTa          | Pretrained Model  | 96.73        | 95.79        |  

## References  
1. **POS Tagged Nepali Corpus**:  
   - Developed by the **Center for Research in Urdu Language Processing (CRULP)**.  
   - Derived by translating **100,720 English words** and **4,325 sentences** from the **PENN Treebank**, provided by the **Linguistic Data Consortium (LDC)**. 

2. **Word2Vec**:  
   - [Nepali Word2Vec Embedding](https://github.com/nowalab/nepali-word-embeddings/tree/master/word2vec).

3. **NepBERTa**:  
   - [Nepali BERT Model](https://github.com/ashishpatel26/nepberta).  



