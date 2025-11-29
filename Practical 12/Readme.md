# Metropolis Algorithm vs Deterministic Model

## 1. Aim
The aim of this experiment is to implement the **Metropolis algorithm (Monte Carlo method)** to estimate the statistical properties of a standard normal distribution and compare the obtained results with a **deterministic (analytical) model**. The objective is to study how stochastic sampling approximates exact theoretical values.

---

## 2. Technologies Used
- Python 3  
- NumPy (numerical computations)  
- Math (mathematical functions)  
- Matplotlib (visualization of results)

---

## 3. Explanation of Both Parts

### PART A: Metropolis Algorithm (Monte Carlo Model)
The Metropolis algorithm is a **Markov Chain Monte Carlo (MCMC)** method used to sample from a probability distribution when direct sampling is difficult.

- A target distribution is chosen (standard normal distribution).
- A new sample is proposed using a normal proposal distribution.
- The proposed sample is accepted or rejected based on an acceptance probability.
- After discarding initial samples (burn-in), the remaining samples are used to estimate:
  - Mean
  - Variance

This method provides approximate results due to its stochastic nature.

---

### PART B: Deterministic Model
The deterministic model uses **analytical formulas** of the standard normal distribution.

For a standard normal distribution:
- Mean = 0
- Variance = 1

These values are exact and do not involve randomness or sampling.

---

## 4. Results and Discussion

### Metropolis Algorithm Results:
- Estimated Mean ≈ 0.0124  
- Estimated Variance ≈ 0.9900  
- Acceptance Rate ≈ 0.7074  

### Deterministic Model Results:
- True Mean = 0.0000  
- True Variance = 1.0000  

### Error Analysis:
- Mean Error = 0.0124  
- Variance Error = 0.0100  

The Monte Carlo estimates are very close to the analytical values, with minor differences due to random sampling and finite sample size.

---

## 5. Conclusion
The Metropolis algorithm successfully approximates the target distribution and produces results that closely match the deterministic analytical model. Small deviations in the estimated mean and variance are expected due to the stochastic nature of Monte Carlo methods. As the number of samples increases, these errors decrease and the Monte Carlo estimates converge to the deterministic values, validating the effectiveness of the Metropolis algorithm.

---
