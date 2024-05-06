# reviews_text_classification
This repo includes work on topic modelling and multi-text classification using HuggingFace Setfit Method. The aim is to test two different approaches:
- 1)  Classic Topic Modelling: to uncover recurring themes and trends within customer comments using generative probabilistic modelling approach mainly LDA (Latent Dirichlet Allocation) from gensim and scikit-learn. Two feature engineering techniques were tested: Bag of words and TF-IDF (Term Frequency and Inverse Document Frequency).
- 2)  SetFit Few-Shot Learning : to fine-tune a HuggingFace (HF) sentence transformers model with minimal data to automatically categorise and label reviews.

* The project is applied on a public dataset of British Airways customers reviews taken from [Kaggle](https://www.kaggle.com/datasets/okechukwuobiahu/british-airways-reviews/data)
        
## The repo structure is as follows: 
