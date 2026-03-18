# Bayes Theorem — Loan Dataset Analysis

A statistical analysis applying Bayes Theorem to a real-world loan dataset, exploring two conditional probability hypotheses and verifying results against direct probability calculations.

**Dataset:** [Loan Data Set](https://www.kaggle.com/datasets/burak3ergun/loan-data-set) (Kaggle) — 614 observations, 13 variables

---

## Overview

This project uses Bayes Theorem to answer two questions about loan applicants:

1. **Given that an applicant is married, what is the probability they live in a rural area?**
2. **Given that an applicant is a college graduate, what is the probability their loan gets approved?**

Each hypothesis was tested using both a direct conditional probability calculation and Bayes Theorem, then evaluated on support and confidence.

---

## Results

| Hypothesis | Direct P | Bayes P | Support | Confidence |
|---|---|---|---|---|
| P(Rural \| Married) | 0.2915 | 0.2915 | 18.99% | HIGH |
| P(Loan Approved \| Graduate) | 0.7083 | 0.7083 | 55.37% | VERY HIGH |

**Key findings:**
- Both methods produced identical results, confirming the calculations
- Graduates have a ~71% loan approval rate, supported by over half the dataset
- Married applicants have a ~29% chance of being in a rural area — moderate but credible with 116 joint observations

---

## Tools

- **Language:** R
- **Methods:** Conditional probability, Bayes Theorem, support & confidence assessment

---

## Formula Used

```
P(E|H) = P(H|E) × P(E) / P(H)
```

Where H is the hypothesis (e.g. applicant is married) and E is the evidence (e.g. rural property area).
