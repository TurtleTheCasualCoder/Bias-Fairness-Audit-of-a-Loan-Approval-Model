## This project evaluates gender-based fairness in a binary loan approval model rather than focusing solely on accuracy, the analysis examines error distribution across demographic groups to identify potential algorithmic bias.

# Dataset

Source: Public loan approval dataset (Kaggle)

Target variable: Loan approval (Approved / Not Approved)

Sensitive attribute: Gender

The dataset contains a significant class imbalance, with male applicants forming the majority.

# Methodology

Data cleaning and preprocessing

Encoding categorical features

Logistic Regression model training

Group-wise evaluation using:

False Positive Rate (FPR)

False Negative Rate (FNR)

Approval rate comparison

# Key Findings

Female applicants showed zero false negatives, indicating no eligible female applicants were wrongly rejected.

Female applicants exhibited a higher false positive rate, suggesting a tendency toward incorrect approvals for the  group.

Overall approval rates were similar across genders.

# Important Context

The female subgroup had a small sample size, making fairness metrics sensitive to minor changes.

Zero error does not imply fairness, but may reflect limited representation.

Bias analysis requires examining error patterns, not just outcomes.

# Lessons Learned

Bias does not always appear where expected.

Dataset imbalance significantly affects fairness metrics.

Responsible model evaluation goes beyond accuracy scores.

# Future Improvements

Apply resampling techniques to stabilize subgroup metrics

Evaluate additional fairness metrics (Equal Opportunity, Demographic Parity)

Compare results across different models

# Tools & Technologies

Python

Pandas, NumPy

Scikit-learn

# Conclusion

This project demonstrates the importance of critical evaluation in machine learning, especially when models are used in decision-making systems that affect people.

# Author
TurtleTheCasualCoder
(anshul)
