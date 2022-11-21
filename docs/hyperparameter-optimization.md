# Baseline Semantic Segmentation on Satellite Images

## Hyperparameter Optimization

### BOHB

    What is BOHB?
    BO is an abbreviation for “Bayesian Optimization” and HB is an abbreviation for “Hyperband”. BOHB depends on HB (Hyperband) to decide how many configurations to assess with which budget, but it substitutes a model-based search for the initial random pick of configurations made by HB at the start of each iteration (Bayesian Optimization). The typical consecutive halving approach is used with these configurations after the desired number of configurations for the iteration has been attained. In order to serve as the foundation for our models in subsequent iterations, we keep track of the performance of all function evaluations g(x, b) of configurations x on all budgets b.
