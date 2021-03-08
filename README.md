# uplift_modelling

This is a repo that explores various uplift modelling packages on the [Criteo dataset](http://ailab.criteo.com/criteo-uplift-prediction-dataset/). 
- Note that the exact Criteo dataset is too large (3.2 GB) so it was not pushed into the repo.
- A subsample (1%) of the data with Stratified train-test split was done, and can be replicated using the [Notebook code found in the Criteo Data folder](https://github.com/kfoofw/uplift_modelling/blob/master/criteo_data/Reproducible%20data%20splitting.ipynb)

The concept of __uplift__ is based on the concept of __heterogenous treatment effects within experimental units in a population__. With uplift, we can create policies for targeted treatment for specific populations that respond best to the treatment, or avoid wasting resources applying treatment to population subgroups that do not respond well to it. In the context of digital commerce, we can decide prioritise customer segments to perform targeted campaign advertising/coupons, and perform benefit-cost optimisation for campaigns.

All of this is centered around __causal inference__, and without going into too much details, there are some assumptions we need to make about the causal model:
- Unconfoundedness
- Conditional exchangeability
- No collider bias

Some concepts that will be explored in this repo are:
- Gain/Qini curves
- Propensity Scoring
- Transformed Outcomes
- Meta-Learners
- CausalForests

### Jupyter Notebooks Links
- [Criteo modelling with Pylift](https://github.com/kfoofw/uplift_modelling/blob/master/pylift/Criteo%20modelling%20with%20Pylift.ipynb)
- [Criteo modelling with Meta Learners (S, T, X)](https://github.com/kfoofw/uplift_modelling/blob/master/meta_learners/Criteo%20modelling%20with%20Meta%20Learners%20(S%2C%20T%2C%20X).ipynb)

### Packages explored:
- [Pylift](https://pylift.readthedocs.io/en/latest/)
- [CausalML](https://causalml.readthedocs.io/en/latest/)
- [EconML](https://econml.azurewebsites.net/)


### Repo Usage

To test out this repo, it would be best to create a virtual env with Python 3.6 for this repo. Once you have created the necessary environment, you can proceed to install the required software packages from the "requirements.txt" file found at the root of the repo.

```pip install requirements.txt```

