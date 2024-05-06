# reviews_text_classification
This repo includes work on topic modelling and multi-text classification using HuggingFace Setfit Method. The aim is to test two different approaches:
- 1)  Classic Topic Modelling: to uncover recurring themes and trends within customer comments using generative probabilistic modelling approach mainly LDA (Latent Dirichlet Allocation) from gensim and scikit-learn. Two feature engineering techniques were tested: Bag of words and TF-IDF (Term Frequency and Inverse Document Frequency).
- 2)  SetFit Few-Shot Learning : to fine-tune a HuggingFace (HF) sentence transformers model with minimal data to automatically categorise and label reviews.

* The project is applied on a public dataset of British Airways customers reviews taken from [Kaggle](https://www.kaggle.com/datasets/okechukwuobiahu/british-airways-reviews/data)
        
## The repo structure is as follows: 
- data:
  - labelled_reviews.csv: includes a small sample of labelled reviews across 6 business themes (8 labelled reviews by class)
  - reviews.csv: represents the raw data of all customers reviews
 
- src:
  - topic_modelling.py: sample Python script of topic modelling notebook.
 
- notebooks:
  - customers_reviews_topic_modelling.ipynb: includes the whole topic modelling work; from data preprocessing to feature engineering, LDA model training, topics visualisations and topics selection.
  - sample_example_finetuning_setfit.ipynb: includes a simple notebook to fine-tune a setfit model quickly using a sample data from Datasets library
  - customers_reviews_finetuning_setfit.ipynb: includes fine-tuning a setfit model on a small labelled of customers reviews
  - customers_reviews_inference_setfit.ipynb: includes the process to use the fine-tuned model to generate inference on unseen datapoints and applying evaluation/monitoring mechanism using text similarity algrothims.
- README.md: a detailed description of project files.

## Python Packaging:
- Follow the pip installs within each notebook
- Libraries and packages needed:
  - python >=3.8
  - pandas=1.5.3
  - re=2.2.1
  - setfit=1.0.3
  - fuzzywuzzy=0.18.0
  - loguru=0.6.0
  - datasets=2.11
  - nltk=3.8.1
  - sklearn=1.2.2
  - gensim=4.3.2
  - wordcloud==1.9.3
