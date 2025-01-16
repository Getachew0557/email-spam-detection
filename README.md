# Bayesian Email Spam Detection

This project implements a Bayesian classifier to detect spam emails using the **SMS Spam Collection Dataset** from UCI. It includes preprocessing, calculation of priors, likelihoods, posterior probabilities, and metrics such as **Precision**, **Recall**, and **F1-Score** to evaluate performance.

## Features

- Bayesian Decision Theory applied for spam detection.
- Priors and likelihoods calculated with Laplace smoothing.
- Posterior probabilities computed using Bayes' theorem.
- Performance metrics: Precision, Recall, and F1-Score.
- SMS Spam Collection Dataset preprocessing and analysis.

## Dataset

The project uses the **SMS Spam Collection Dataset** available from UCI, which contains labeled messages (`spam` or `ham`).

## Requirements

- Python 3.7+
- Libraries:
  - pandas
  - numpy
  - scikit-learn

Install the required libraries using:

```bash
pip install -r requirements.txt
```
## How It Works
#### Data Preprocessing:

Text messages are converted to lowercase and split into individual words.
Priors Calculation:

The prior probabilities of a message being spam or ham are calculated based on the training data.
Likelihood Calculation:

Using Laplace smoothing, likelihood probabilities for each word are computed for both spam and ham classes.
Posterior Probabilities:

Bayes' theorem is used to compute the probabilities of a message being spam or ham given the occurrence of specific words.
Classification:

Messages are classified as spam or ham based on the higher posterior probability.
Performance Metrics:

Evaluate the classifier using Precision, Recall, and F1-Score.

## Documentation
- Read the documentation on `/Documentation/Bayesian_spam_detection.pdf`