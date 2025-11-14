AI DRIVEN LOAN RECOVERY 

What this project does (in one line): A production-minded, two-stage ML workflow that predicts which delinquent loans are recoverable and, if recoverable,which are likely to be fully vs. partially recovered; so collections teams deploy the right action at the right cost (e.g., a $10 call vs. a $500 legal notice).

Why it matters (business impact):

- Banks lose up to 7% of their loan portfolio during economic downturns due to poor recovery targeting, so improving recovery decisions directly protects revenue and reduces charge-offs.
 
 - The model helps collections teams recover more debt at a lower cost by identifying which accounts are worth pursuing and recommending the least costly effective action (e.g., call vs. legal notice).

 - Cost-sensitive design reduces expensive false positives, ensuring staff time and operational budgets are deployed where they generate the highest return.

 - The workflow aligns with FCAC/PIPEDA, enabling financial institutions to use AI-driven recovery strategies without compromising compliance or customer fairness.
   
What I built (high level):

Two-step classifier on historical loans dataset:

  - Recovered vs. Written-off (ROC AUC ≈ 0.76, precision up to 0.95 on “recovered”).
  - Fully vs. Partially Recovered (ROC AUC ≈ 0.81, precision ≈ 0.85 on “fully”).

End-to-end pipeline: EDA → cleansing → feature engineering → class balancing (SMOTE) → model selection → policy-ready recommendations.

Models: Logistic Regression (forward/stepwise selection) guided by Random Forest feature importance; emphasis on interpretability for operations.

Actionable predictors surfaced (e.g., payment history, collection attempts, settlement offers) to re-strategise loan recovery.

 Recommendations 
   - Implement loyalty-based retention programs (e.g., interest rate incentives, fee waivers) to maintain high repayment rates while minimizing collection cost
   - Incorporate settlement-based recovery strategies, especially for delinquent accounts flagged as having moderate recovery potential,to increase resolution
     rates while reducing prolonged collection costs.
   - Introduce stricter credit assessments and collateral backed lending for new business loans . For existing high risk accounts, apply early settlement
   - negotiations to mitigate write-offs  



methods: Python (pandas, scikit-learn), class balancing (SMOTE), AUC/Precision/Recall/F1, odds-ratio interpretation, dashboard-ready outputs for operation

/notebooks: EDA, feature selection, modelling which includes decison trees, Random Forest importance, forward,backward and stepwise LR, 
/reports: Analytic plan, Documentation, loan recovery executive overview, monitoring and governance. 



/reports: Analytic plan, Documentation, loan recovery executive overview, monitoring and governance.
