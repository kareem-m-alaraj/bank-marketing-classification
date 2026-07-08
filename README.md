# Bank Term Deposit Subscription Prediction

Binary classification project (CS417 Introduction to Data Mining, IUS) predicting whether a client subscribes to a term deposit, using the UCI Bank Marketing dataset (~45,000 records, 16 attributes).

## Team
Abdalkarim Alaraj, Muhamed Maglić, Hamza Hubanić — supervised by Prof. Emine Yaman

## Highlights
- Compared 5 classifiers: Decision Tree, Naive Bayes, k-NN, Random Forest, Logistic Regression
- Full preprocessing pipeline: leakage removal (`duration`), sentinel handling (`pdays`), one-hot encoding, stratified 75/25 split, feature scaling
- Naive Bayes achieved the best F1/recall (0.409 / 0.424) for identifying subscribers; Random Forest achieved the best ROC-AUC (0.771) for ranking clients
- Class-weighted variants raised Logistic Regression recall from 18% to 60%
- K-Means clustering + Random Forest feature importance for interpretability

## Files
- `notebook/` — full analysis (EDA, preprocessing, modeling, clustering)
- `paper/` — IEEE-format paper with results and discussion

## Report
See [`paper/CS417_BankMarketingProjectPaper.pdf`](paper/CS417_BankMarketingProjectPaper.pdf) for full methodology and results.
