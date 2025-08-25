AI-Driven Loan Recovery (2-Step Predictive Model) — Repository Overview

What this project does (in one line):
A production-minded, two-stage ML workflow that predicts which delinquent loans are recoverable and, if recoverable, which are likely to be fully vs. partially recovered—so collections teams deploy the right action at the right cost (e.g., a $10 call vs. a $500 legal notice).

Why it matters (business impact):

Targets higher recovery rates and lower operating costs by prioritizing the right accounts and strategies.

Designed around cost-sensitive precision to avoid expensive false positives and misallocated effort.

Built with regulatory awareness (FCAC/PIPEDA): sensitive attributes excluded, transparent modeling choices.

What I built (high level):

Two-step classifier on 500 historical loans:

Recovered vs. Written-off (ROC AUC ≈ 0.76, precision up to 0.95 on “recovered”).

Fully vs. Partially Recovered (ROC AUC ≈ 0.81, precision ≈ 0.85 on “fully”).

End-to-end pipeline: EDA → cleansing → feature engineering → class balancing (SMOTE) → model selection → policy-ready recommendations.

Models: Logistic Regression (forward/stepwise selection) guided by Random Forest feature importance; emphasis on interpretability for operations.

Actionable predictors surfaced (e.g., payment history, collection attempts, settlement offers) to re-strategise loan recovery.


Tech & methods: Python (pandas, scikit-learn), class balancing (SMOTE), AUC/Precision/Recall/F1, odds-ratio interpretation, dashboard-ready outputs for operations.

Repository highlights:

/notebooks: EDA, feature selection, modelling which includes decison trees, Random Forest importance, forward,backward and stepwise LR,

/reports: Analytic plan, Documentation, loan recovery executive overview, monitoring and governance.
