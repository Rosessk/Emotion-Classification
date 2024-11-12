# Emotion-Classification

This analysis is divided into two main parts to compare the results of Neural Network-Based Methods and non-Neural Network-Based Methods.

1. Using Logistic Regression for Tweet Classification

Since LR is non-neural, extensive preprocessing is required. Steps include lemmatisation or stemming and adding negation negate sequences to make the BoW could identify negative feelings different from positive feelings. Features include TF-IDF vectorisation tested on bigrams and unigrams, along with lexicon-based features.

2. Using Bidirectional Encoder Representations from Transformers (BERT) and TinyBERT for Tweet Classification

- Fine-tuning BERT-based and TinyBERT models specifically for the Emotion-Classification task.
- Configuration and Hyperparameter Tuning. For BERT-based and TinyBERT models, two hyperparameters are tuned: batch size and learning rate.
- As these models are pretrained, extensive preprocessing isn’t necessary.
- The AutoTokenizer from the Hugging Face library is used to convert text into the appropriate format for BERT-based and TinyBERT models.
