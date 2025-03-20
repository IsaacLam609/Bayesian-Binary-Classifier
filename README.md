# Bayesian Binary Classifier
This code implements a Bayesian binary classifier using logistic regression with the Laplace approximation. The key steps in the implementation are:

1. Feature Expansion: transforms input data using Radial Basis Functions (RBFs).
2. MAP Estimation: computes the Maximum A Posteriori (MAP) estimate by optimizing the negative log-posterior with a Gaussian prior on model parameters.
3. Laplace Approximation: approximates the posterior distribution as a Gaussian centered at the MAP estimate.
4. Predictive Distribution: uses the Laplace approximation to make predictions with uncertainty quantification.
5. Model Evidence Optimization: uses grid search to optimize prior variance and RBF width by maximizing model evidence. Results are visualized using a heat map.
6. Evaluation & Comparison: computes predictive distribution, log-likelihoods and confusion matrices for MAP and Laplace solutions with different values of hyperparameters.
