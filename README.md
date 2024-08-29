# README for Offensive Speech Classification Study

## Overview

This repository contains the code and documentation for the study titled "Offensive Speech Classification Study" conducted by Nerry Asyncrite Koukoui. The research focuses on the detection and classification of offensive language in user-generated content from various online platforms, utilizing the Offensive Language Identification Dataset (OLID).

## Abstract

The study addresses the increasing prevalence of offensive content on social media and other platforms. It reviews existing research on identifying types of offensive content, including hate speech and cyberbullying. The paper emphasizes the importance of detecting offensive language to maintain a safe online environment.

## Materials

- **Code**: The implementation of the models and analysis is provided in the Jupyter Notebook linked above.

## Model Selection

### Summary of Selected Models

1. **Stochastic Gradient Descent (SGD) Classifier**
   - A machine learning algorithm effective for multi-class classification tasks, particularly in Natural Language Processing (NLP).
   - Operates by minimizing a loss function to predict class labels.

2. **Recurrent Neural Networks (RNN)**
   - Suitable for handling sequential data, RNNs maintain memory of previous inputs, making them effective for tasks like text classification.
   - **Long Short-Term Memory (LSTM)** networks are a variant of RNNs that excel in capturing long-term dependencies.

### Justification of Model Selection

- **SGD Classifier**: Chosen for its simplicity, interpretability, and efficiency with large datasets. It is particularly useful in NLP applications.

- **RNNs**: Selected for their ability to model sequential data and capture context, which is crucial for understanding the meaning of sentences in offensive speech classification.

## Design and Implementation of Classifiers

### Key Parameters

- **Learning Rate**: Determines the step size during training.
- **Dropout Rate**: Regularizes the model to prevent overfitting in RNNs.
- **Batch Size**: Affects training speed and model quality.
- **Number of Epochs**: Defines how many times the model is trained on the dataset.
- **Hidden Layer Size**: Influences model complexity and capacity.
- **Loss Function**: For binary classification, Binary Cross-Entropy Loss is used.
- **Optimizer**: Algorithm used to update model weights during training.

## Dataset

The OLID dataset is utilized for training, validation, and testing, with the following distribution:

| Subset | Total Tweets | % Offensive | % Non-Offensive |
|--------|--------------|-------------|------------------|
| Train  | 12,313       | 33.2%       | 66.8%            |
| Valid  | 927          | 33.24%      | 65.75%           |
| Test   | 826          | 29.06%      | 75.06%           |

## Model Performance

Performance metrics, including F1-scores, are provided to evaluate the effectiveness of the models across different data sizes. The results indicate that:

- **Model 1** shows a tendency to overfit smaller datasets.
- **Model 2** demonstrates robustness and consistent performance across varying data sizes, although it struggles with certain classification tasks.

## Findings and Conclusion

The study concludes that both the SGD Classifier and RNNs have unique advantages for offensive speech classification. The choice of model should consider the specific requirements of the task, including the nature of the data and the importance of interpretability versus performance.

## References

A list of references is included in the study, highlighting key research and methodologies relevant to offensive speech detection.

---

This README serves as a comprehensive guide to understanding the objectives, methodologies, and findings of the Offensive Speech Classification Study. For further details, please refer to the linked Jupyter Notebook.

Citations:
[1] https://colab.research.google.com/drive/1H9RAweuQ-6s4cnEx_0_NJhZpNSdNmhMr
