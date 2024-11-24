Here is the updated `README.md` file reflecting the use of the Jupyter Notebook file:

---

### README.md

# Assignment: Causality in Data Mining

This repository contains solutions and explanations for **Exercise Sheet 3: Causality** from the Data Mining course at the University of Vienna, Winter Semester 2024/25. The assignment explores concepts of causality using statistical methods, with a focus on Granger causality, multivariate causal models, and bivariate additive noise models.

---

## Assignment Overview

### **Exercise 3-1: Granger Causal Test (6 points)**  
The objective is to analyze causal relationships between variables using Granger causality with real-world data on chickens (\(Y\)) and eggs (\(X\)) from U.S. egg production (1930–1935).

1. **Auto-regression for \(X\) and \(Y\) (1.5 points)**  
   Compute regression coefficients \((\beta_0, \beta_1, \beta_2)\) for predicting \(Y\) based on lagged values of \(X\) and \(Y\). Compute \(RSS1\) (Residual Sum of Squares for the full model).

2. **Auto-regression without \(Y\) (1.5 points)**  
   Repeat the regression excluding \(Y\) and compute \(RSS2\) (Residual Sum of Squares for the reduced model).

3. **Statistical Test (1.5 points)**  
   Use the Granger-Sargent test to determine if \(X\) Granger-causes \(Y\) with \(\alpha = 0.05\).

4. **Causal Test for the Reverse Direction (1.5 points)**  
   Repeat the above steps to test if \(Y\) Granger-causes \(X\). Interpret the results to address the "chicken or egg" question.

---

### **Exercise 3-2: Multivariate Granger Model (2 points)**  
Analyze causal relationships in high-dimensional settings using multivariate Granger models.

1. **Consistency of Granger Models (1 point)**  
   Evaluate the consistency of causal inference with ordinary least squares and adaptive Lasso penalties. Discuss if the method generalizes well in high-dimensional data.

2. **HMMLGA Algorithm (1 point)**  
   Explain the **High-order Mixed Model Lasso Granger Algorithm (HMMLGA)** and describe its key hyperparameters, including regularization parameter \((\lambda)\), lag order \((d)\), and stopping criteria.

---

### **Exercise 3-3: Bivariate Causal Models on Non-Temporal Data (2 points)**  
Explore causal relationships using bivariate additive noise models.

1. **Non-identifiability in Linear-Gaussian Cases (1 point)**  
   Explain why causal relationships between variables \(X\) and \(Y\) are non-identifiable when the noise is Gaussian and relationships are linear. Discuss the role of symmetry in the joint distribution.

2. **Causal and Anti-Causal Directions (1 point)**  
   For \(X =\) age and \(Y =\) blood pressure, explain:
   - How to change \(P(\text{effect}|\text{cause})\) without affecting \(P(\text{cause})\).
   - How to change \(P(\text{cause})\) without affecting \(P(\text{effect}|\text{cause})\).
   - Challenges in the anti-causal direction.

---

## Key Topics Covered

- **Granger Causality**:
  - Statistical framework for analyzing temporal causal relationships.
  - Tests based on differences in residual sums of squares.
- **Multivariate Granger Models**:
  - Extensions to handle high-dimensional data with sparse penalties like Lasso.
- **Bivariate Additive Noise Models**:
  - Challenges of causal inference in non-temporal, symmetric distributions.
- **Real-World Applications**:
  - Example datasets and domain-specific interpretations (e.g., chickens and eggs, age and blood pressure).

---

## Repository Structure

```plaintext
├── Exercise_Sheet_3_Solution.ipynb  # Jupyter Notebook containing all solutions
├── README.md                        # Overview of the assignment
```

---

## Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/username/causality-assignment.git
   cd causality-assignment
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the solutions:
   Open the Jupyter Notebook in your preferred environment (e.g., Jupyter Lab or Jupyter Notebook):
   ```bash
   jupyter notebook Exercise_Sheet_3_Solution.ipynb
   ```
   - **Exercise 3-1**: Granger causality tests.
   - **Exercise 3-2**: Multivariate Granger models.
   - **Exercise 3-3**: Bivariate additive noise models.

---

## Acknowledgments

This assignment is part of the **Data Mining** course at the University of Vienna, guided by **RNDr. Katerina Schindlerová, CSc., Privatdoz.** and **Pranava Mummoju, MSc.**.

