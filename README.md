# Predictive Modeling for Multi-Label Tagging in Algorithmic Challenges

## Overview
This project aims to enhance user interaction with CodeForce, a hub for algorithmic contests, by developing a predictive framework that assigns multiple descriptive labels to each posted problem based on its textual content. By parsing problem descriptions and assessing various computational models, including logistic regression, random forest classifiers, and BiLSTM networks, the study seeks to refine the tagging mechanism, significantly improving accuracy and reducing misclassification to help users find relevant problems that match their proficiency and search requirements.

## Dataset
Our research relied on a comprehensive dataset sourced from Kaggle, originally obtained from Codeforce's online programming competitions. The dataset comprises four columns: 'contest', 'problem name', 'problem statement', and 'problem tags', with a total of 8,434 entries. The key columns for our research are 'problem statement' and 'problem tags', which are crucial for the tagging mechanism.

## Data Architecture
The dataset was meticulously organized and preprocessed to ensure effective model training. During preprocessing, elements such as HTML codes, LaTeX symbols, stop words, non-ASCII characters, digits, and punctuation were removed. Text normalization techniques, including lemmatization and stemming, were applied to improve data consistency.

## Tools Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- PyTorch

## Methods
The project utilized a combination of machine learning and deep learning techniques to categorize programming problem statements into their respective tags.

### Algorithms
- **Logistic Regression with One-vs-Rest Classification**
- **Random Forest Classifier with One-vs-Rest Classification**
- **Bi-Directional LSTM (Bi-LSTM)**
- **SGDClassifier with One-vs-Rest Classification**

## Results
The analysis indicated varying performance levels across different algorithms:
- **Logistic Regression**: Achieved a micro F1 score of 0.37.
- **SGDClassifier**: Achieved a micro F1 score of 0.37.
- **Random Forest Classifier**: Underperformed with an F1 micro score of 0.08.
- **Bi-Directional LSTM**: Yielded an F1 score of 0.27 after 40 epochs.

## Outcome
The investigation revealed that machine learning models, especially Logistic Regression, performed well on the dataset. Although deep learning techniques showed potential, their performance was hampered by limited data. Future research should focus on collecting more diverse data or employing data augmentation techniques to enhance model performance. Advanced text embeddings like BERT and XLNet could also be explored to further improve classification results in subsequent studies.
