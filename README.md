# Machine Learning: SVMs, Generative Models & EM

Three end-to-end machine learning projects from **CS771: Introduction to Machine Learning** at **IIT Kanpur** (2025–26), covering supervised classification, probabilistic generative modelling, and unsupervised mixture regression.



## Projects

### 1. [SVM Hyperparameter Sensitivity Analysis](./Assignment_1)
- Proved that synthetically generated multi-class data is **always linearly separable** via geometric margin analysis
- Systematically studied how regularisation **C**, stopping tolerance, max iterations, and loss function affect **LinearSVC** performance across three difficulty regimes (low / medium / high challenge)
- Quantified the **bias-variance tradeoff**: hyperparameter sensitivity scales monotonically with inter-class margin width

**Topics:** Linear SVMs · Regularisation · Optimisation · Bias-Variance Tradeoff

### 2. [Bayesian Image Reconstruction on MNIST](./Assignment_2)
- Derived a **single-step joint MAP inference** procedure for classifying and reconstructing MNIST digits with missing pixels under per-class Gaussian generative models
- Leveraged **Schur complement** decomposition of the covariance matrix to obtain a closed-form classification objective with a reconstruction-uncertainty penalty
- Implemented **naive** and **numerically-stabilised** (Tikhonov + eigenvalue-clipped) variants; naive single-step outperforms the two-step baseline by **0.44%** under light censoring (2–8% missing pixels)

**Topics:** Gaussian Generative Models · MAP Inference · Bayes' Rule · Schur Complement · Numerical Stability

### 3. [EM Mixture Regression for Air Quality](./Assignment_3)
- Applied the **EM algorithm** to learn a mixture of Ridge regressors for predicting ground-level ozone concentrations from low-cost sensor data
- Conducted **convergence analysis**, **model complexity selection** (optimal K=4 components), and **feature ablation** identifying temperature as the dominant predictor (+5.42 MAE impact)
- Compared against **DecisionTreeRegressor** baselines — mixture model achieves competitive MAE ≈ 10.69 while providing interpretable component specialisation across pollution regimes

**Topics:** EM Algorithm · Mixture Models · Ridge Regression · Feature Importance · Decision Trees


## Authors

**Group: Deepminds** — CS771, IIT Kanpur (2025–26)

---

Each assignment includes a full **NeurIPS-style report** (LaTeX) with mathematical derivations, experimental results, and analysis.
