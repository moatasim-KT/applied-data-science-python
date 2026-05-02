
## Practice
Choose a classification dataset on [Kaggle](https://www.kaggle.com/datasets) and build a complete machine learning pipeline using Scikit-Learn. Ensure your pipeline includes automated steps for feature engineering, scaling, and training, and utilize cross-validation to assess performance accurately.
# Week 9: Scikit-Learn - Pipelines & Preprocessing

## Overview
Machine learning is not just about the algorithm; it's about the data pipeline. This week focuses on automating the sequence of transformations required to prepare data for modeling, ensuring reproducibility and preventing data leakage.

## Key Concepts
### 1. The Estimator API
- **Consistent Interface**: Scikit-Learn uses a uniform interface (`fit`, `predict`, `transform`) for all estimators, which makes swapping models and pre-processing steps straightforward.
- **Fitting vs. Transforming**: Understanding that `fit` learns parameters from training data (like mean or variance) and `transform` applies those parameters to new or test data is crucial to prevent leakage.

### 2. Pipelines
- **Reproducibility**: Pipelines bundle together sequential data processing steps and a final machine learning model into a single estimator object. This guarantees that the exact same transformations (e.g., scaling) applied to the training set are correctly applied to the test or production data.
- **Data Leakage Prevention**: Pipelines make it difficult to accidentally fit a pre-processor on the test set, ensuring valid performance evaluation.
