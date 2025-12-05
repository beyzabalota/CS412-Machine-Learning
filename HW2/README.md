# CS412 – Machine Learning  
## Homework 2: MLE, MAP, and Probabilistic Analysis  
**Semester**: Spring 2024  
**Student**: Beyza Balota, 31232  
**Date**: 04.04.2024  

---

## Overview

This homework consists of two major parts:

### Part 1 – Maximum Likelihood Estimation (MLE) & Maximum A Posteriori (MAP)  
In this section, we model the flight flutteriness of butterflies using the **Fluter distribution** (a synthetic probability distribution). The task involves:
- Deriving the MLE estimator for the distribution's parameter α
- Computing the MAP estimator given a specific prior
- Explaining each mathematical step in detail and using symbolic computation where needed

### Part 2 – Bayesian Probability Analysis on Real-World Survey Data  
In this part, we perform probabilistic reasoning using the **2017 Kaggle Machine Learning and Data Science Survey** dataset. Key tasks include:
- Estimating conditional and joint probabilities from real data
- Applying **Bayes' Theorem** for reverse probability inference
- Working with multiple CSV files and cross-referencing them (e.g., salary, country, tools used)

---

## Files

```
CS412-HW2/
├── cs412_hw2_notebook.ipynb        # Main notebook with code, math, and answers
├── multipleChoiceResponses.csv     # Main responses file (provided)
├── conversionRates.csv             # Currency conversion file (provided)
├── schema.csv                      # Column explanations (referenced only)
├── README.md                       # This file
```


---

## Methods Used

### Part 1 – MLE & MAP
- Symbolic derivations for:
  - Likelihood function
  - Log-likelihood
  - Posterior distribution
- Used mathematical simplification to derive closed-form estimators

### Part 2 – Probabilistic Data Analysis
- Python `pandas` used for:
  - Filtering based on conditions
  - Merging and cleaning large-scale survey data
  - Group-based aggregation and conditional counting
- Used `conversionRates.csv` to normalize salaries into USD
- Addressed questions involving conditional probability, joint probability, and Bayes' Theorem

---

## Example Questions Solved
- What’s the probability a C/C++ user is a Programmer?
- What’s the probability someone is a Data Scientist given they majored in CS or Math?
- What’s the joint probability of someone being over 30 and having at least a Bachelor’s?
- Applying Bayes’ Theorem:  
  What is the probability someone has a PhD given that they wear glasses?

---

## Libraries Used

- `pandas`
- `numpy`
- `matplotlib` (optional, for plotting)
- No external ML libraries used

---

## Insights

- Most conditional probabilities were computed through direct filtering and ratio of counts
- Bayesian reasoning provided a clear framework for combining prior and conditional beliefs
- Salary data normalization and parsing required careful type conversion and merging

---

## Status

- All 8 sub-questions completed  
- Clean and modular code  
- Annotated calculations and reasoning  
- Real-world dataset exploration

