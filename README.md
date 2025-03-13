# neural-network-challenge-2

Briefly answer the following questions:

1. Is accuracy the best metric to use on this data? Why or why not?

- Accuracy isn’t necessarily the best metric for this dataset because attrition is often imbalanced. This means the number of employees who leave versus those who stay can differ substantially. In imbalanced classification, metrics like precision, recall, the F1-score, or    AUC provide a clearer picture of model performance.

2. What activation functions did you choose for your output layers, and why?

- This notebook uses a sigmoid activation function for the Attrition branch and a softmax activation function for the Department branch. Sigmoid is a good choice for binary classification because it outputs probabilities between 0 and 1, while softmax is appropriate for      multi-class problems because it normalizes outputs into probability distributions across multiple categories.

3. Can you name a few ways that this model might be improved?

- Several improvements could be made, including:

  - Feature Engineering: Exploring additional relevant features or transforming existing ones to better capture patterns in the data.
  - Handling Imbalanced Data: Using techniques such as oversampling the minority class, undersampling the majority class, or applying SMOTE (Synthetic Minority Over-sampling Technique).
  - Hyperparameter Tuning: Optimizing parameters like learning rate, number of layers, and dropout rates using grid search or random search.
  - Alternative Models: Experimenting with different architectures and boosting methods (such as XGBoost).
