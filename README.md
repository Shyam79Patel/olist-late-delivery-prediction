# Predicting Late Delivery Risk in E-Commerce Orders

## Problem Statement
Late deliveries negatively impact customer satisfaction and increase operational costs.  
This project predicts whether an order is likely to be delivered late **at the time of purchase**.

## Dataset
Olist Brazilian E-Commerce public dataset.

## Feature Engineering
Features are derived from information available before shipment:
- Order value and item count
- Freight cost and price ratios
- Payment method and installments
- Order time (hour, weekday, month)
- Customer location (state)

## Exploratory Data Analysis
A small set of focused visualizations were used to understand:
- Class imbalance
- Pricing and freight-related risk
- Payment method and time-based patterns

## Models
| Model | ROC-AUC |
|-----|--------|
| Logistic Regression | ~0.60 |
| XGBoost | ~0.725 |

## Inference
The trained pipeline takes raw order-level inputs and outputs the probability of late delivery.

## Limitations & Future Work
- No seller or carrier-level data
- No real-time logistics signals
- Performance limited by public dataset scope
