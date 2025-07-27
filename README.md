# History of Mathematics

This repository supports the Applications chapter from the QMUL booklet **“Laws, Limits, and Randomness: A Mathematical History of Probability”** - to be updated soon. It contains interactive Python examples that demonstrate foundational results like the **Law of Large Numbers (LLN)** and the **Central Limit Theorem (CLT)**, as they emerged through the historical development of probability theory.

[Read the full document (PDF)](https://www.seresearch.qmul.ac.uk/content/pce/ediresources/files/History_of_Maths_QMUL_2024.pdf)

## What’s Included

The `notebook/` includes examples of simulations and visualisations for the following applications in the chapter mentioned:

### Laws of Large Numbers (LLN)
- **Symmetric Random Walk**: Shows how the average position of a *drunk* walker converges to 0.
- **Stochastic Gradient Descent (SGD)**: Demonstrates that even noisy gradients still converge to a global minimum.
- **Markov Chain Monte Carlo (MCMC)**: Empirical Means (after some burn-in samples are removed) converge to Expected Values under repeated sampling - when optimising model parameters.
- **Monte Carlo Integration**: Averages of random function evaluations converge to an integral.

### Central Limit Theorem (CLT)
- **Scaled Random Walk**: Distribution of positions converges to a normal distribution - an introduction to Brownian motion convergence.
- **MCMC Sampling**: Final positions (scaled) of the Markov chain follow a bell curve and a due to CLT Confidence Interval of the error can be calculated.
- **SGD Trajectories**: Parameter updates fluctuate around the optimum in a Gaussian fashion - the core algorithm of Neural Network parameter learning.

### Heavy-Tailed Phenomena
- **St. Petersburg Paradox**: Illustrates when LLN and CLT break down due to infinite expectation - demonstrated the start of utility theory.
- **Comparison with Geometric Game**: Changing the Payoff structure of the game changes the effects of exponential vs. bounded tails.

## Requirements

- Python ≥ 3.7
- NumPy
- Matplotlib
- Jupyter Notebook

## Getting Started

Clone the repo and run the scripts directly, or explore interactively using Jupyter:

```bash
git clone https://github.com/Ivelina0/History-of-Mathematics.git
cd History-of-Mathematics
jupyter notebook
