# CS412 - HW3 Report

**Author:** Beyza Balota  

## Objective

The goal of this assignment is to understand how **learning rate** and **number of iterations** affect training performance. This includes analyzing loss trends, overfitting behavior, and generalization when combining datasets.

## Summary of Results

- **Training Behavior:** Training loss continues to decrease steadily, while validation loss flattens — a sign of mild overfitting.
- **Learning Rate Comparison:**  
  - Large learning rates (e.g., 1e-2) speed up convergence but may overshoot.  
  - Smaller rates (e.g., 5e-4) converge more slowly but more smoothly.
- **Iterations:** Increasing the number of iterations improves performance.
- **Combined Dataset:** When training on all data together, the final loss is lower, indicating improved generalization.

## Files

- `titanicdata.csv`: Dataset used in training.
- `CS412_HW3_Spring2024.pdf`: Assignment instructions.
- `README.md`: This summary report.

