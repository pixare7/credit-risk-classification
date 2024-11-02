# Credit Risk Classification

## Overview

This project aims to build a model that assesses the creditworthiness of borrowers by predicting whether a loan is high risk or healthy. The dataset used includes historical lending information from a peer-to-peer lending service, featuring variables such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. The data was split into training and testing sets, and a logistic regression model was trained on the original data. Predictions were saved, and the model’s performance was evaluated using a confusion matrix and classification report.

## Table of Contents
1. [Overview](#overview)
2. [Results](#results)
3. [Summary](#summary)
4. [Future Work](#future-work)

## Results

#### Figure 1: Classification Report for the Model
![Figure 1](https://github.com/pixare7/credit-risk-classification/blob/main/images/fig1.png)

- **Overall Accuracy**: The model achieved an accuracy of 99%, correctly predicting almost all cases for both healthy and high-risk loans.
- **Precision**:
   - For healthy loans (0): 100% precision, meaning all loans predicted as healthy were indeed healthy.
   - For high-risk loans (1): 87% precision, indicating that 87% of loans predicted as high risk were actually high risk.
- **Recall**:
   - Healthy loans: 100% recall, with all actual healthy loans correctly identified.
   - High-risk loans: 95% recall, with 95% of actual high-risk loans correctly identified.

## Summary

The model accurately predicted nearly all cases of healthy and high-risk loans, demonstrating strong performance, especially in identifying healthy loans. Its ability to correctly classify 100% of healthy loans benefits the lender by minimizing risk. However, with 87% precision in identifying high-risk loans, there is a 13% chance that loans classified as high risk were actually healthy. This misclassification could negatively impact potential borrowers who were declined despite low risk, as well as the lender due to potential business losses from mistakenly excluded applicants.

## Future Work

To further improve this model, we can increase both the volume and quality of the data. Providing a more diverse and balanced dataset would help to reduce overfitting and improve the model’s ability to generalize to new instances, enhancing its predictive accuracy for unseen cases.
