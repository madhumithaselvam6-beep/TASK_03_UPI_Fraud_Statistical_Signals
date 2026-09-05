# UPI Fraud Statistical Signals

## 1. Problem Statement

The objective of this project is to analyze UPI transaction data using statistical methods to identify patterns and signals associated with fraudulent transactions.

The analysis focuses on transaction amount, transaction frequency, transaction timing, device usage, account age, and other behavioral indicators to identify suspicious activities.

## 2. Dataset Description

The dataset contains UPI transaction records with information related to:

- Transaction details
- User and merchant information
- Transaction amount
- Timestamp and transaction time
- Device and IP address information
- Account age
- Transaction velocity
- Authentication behavior
- Location information
- Fraud indicator

The dataset contains 26,393 transactions and 65 original features.

Target variable:

- `is_fraud = 0` → Normal transaction
- `is_fraud = 1` → Fraudulent transaction

## 3. Statistical Methods

The following statistical methods were used:

- Mean
- Median
- Standard deviation
- Quartiles
- Percentiles
- IQR method
- Z-score
- Box plots
- Distribution analysis
- Pattern analysis
- Independent two-sample t-test

The relationship between fraud and transaction amount, transaction velocity, time of day, device usage, and receiver account age was also analyzed.

## 4. Fraud Signal Findings

| Fraud Signal | Fraud Rate | Severity |
|---|---:|---|
| Rapid transaction burst | 100% | Critical |
| New account + large payment | 100% | Critical |
| Unusual device | 100% | Critical |
| High-value transaction | 98.1% | Critical |
| Late-night / early-morning transaction | 29.55% | High |
| Multiple-device usage | 26.86% | High |

### Key Findings

- Average normal transaction amount: approximately 3,620.
- Average fraudulent transaction amount: approximately 10,850.
- Transactions with transaction velocity greater than zero showed a 100% fraud rate in this dataset.
- New receiver accounts combined with large payments showed a 100% fraud rate.
- High-value transactions showed a 98.1% fraud rate.
- Unusual device activity showed a 100% fraud rate.
- Fraud activity was higher during certain early-morning hours.

These percentages describe patterns in this dataset and should not be interpreted as universal guarantees of fraud.

## 5. Visual Analysis

The analysis includes visualizations for:

- Transaction amount distribution
- Fraud vs normal transactions
- Transaction amount box plots
- Outlier analysis
- Transaction velocity vs fraud
- Fraud rate by time of day
- Device usage vs fraud
- Account age vs fraud
- Fraud signal comparison

These visualizations help identify differences between normal and fraudulent transaction behavior.

## 6. Business Recommendations

1. Implement a multi-signal fraud risk scoring system.
2. Generate real-time alerts for rapid transaction bursts.
3. Apply additional verification for new accounts making large payments.
4. Monitor unusual device activity.
5. Monitor repeated late-night or early-morning transactions.
6. Flag unusually high-value transactions for additional verification.
7. Send transactions with multiple fraud signals for manual investigation.
8. Avoid relying on a single fraud indicator when making final decisions.

## 7. Future Scope

Future improvements can include:

- Machine learning-based fraud detection
- Real-time fraud monitoring
- Advanced anomaly detection
- User behavior profiling
- Automated fraud risk scoring
- Feature importance analysis
- Model performance evaluation
- Real-time transaction alert systems
- Continuous monitoring of new fraud patterns

## Conclusion

Statistical analysis identified several strong fraud-related signals, including transaction velocity, unusual device activity, high transaction amounts, and new receiver accounts combined with large payments.

The results demonstrate that statistical analysis can be useful for identifying suspicious transaction behavior and supporting fraud investigation and prevention strategies.
