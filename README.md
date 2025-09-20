# History of Mathematics

This repository supports the Applications chapter from the QMUL booklet **“Laws, Limits, and Randomness: A Mathematical History of Probability”** - final version 2025 now updated. It contains interactive Python examples that demonstrate foundational results like the **Law of Large Numbers (LLN)** and the **Central Limit Theorem (CLT)**, as they emerged through the historical development of probability theory.

[Read the full document (PDF)](https://www.seresearch.qmul.ac.uk/content/pce/ediresources/files/History_of_Maths_QMUL_2025.pdf)

## What’s Included

The `notebook/` includes examples of simulations and visualisations for the following applications in the chapter mentioned:

### Laws of Large Numbers (LLN)
- **Symmetric Random Walk**: Shows how the average position of a *drunk* walker converges to 0.
- **Stochastic Gradient Descent (SGD)**: Demonstrates that even noisy gradients still converge to a global minimum, for convex or pseudoconvex functions - note that most deep learning problems are non-convex and hence converge to the global minimum is not guaranteed. Although [SGD Converges to Global Minimum in Deep Learning via Star-convex Path
](https://arxiv.org/abs/1901.00451#:~:text=2%20Jan%202019%5D-,SGD%20Converges%20to%20Global%20Minimum%20in%20Deep%20Learning%20via%20Star,manner%20to%20a%20global%20minimum.) shows convergene of SGD follows an iterationwise star-convex path in some cases.  
- **Markov Chain Monte Carlo (MCMC)**: Empirical Means (after some burn-in samples are removed) converge to Expected Values under repeated sampling - when optimising model parameters.
- **Monte Carlo Integration**: Averages of random function evaluations converge to an integral.

### Central Limit Theorem (CLT)
- **Scaled Random Walk**: Distribution of positions converges to a normal distribution - an introduction to Brownian motion convergence.
- **MCMC Sampling**: Final positions (scaled) of the Markov chain follow a bell curve and a due to CLT Confidence Interval of the error can be calculated.
- **SGD Trajectories**: Parameter updates fluctuate around the optimum in a Gaussian fashion - the core algorithm of Neural Network parameter learning.

### Heavy-Tailed Phenomena
- **St. Petersburg Paradox**: Illustrates when LLN and CLT break down due to infinite expectation - demonstrated the start of utility theory.
- **Comparison with Geometric Game**: Changing the Payoff structure of the game changes the effects of exponential vs. bounded tails.

### Markov Chain Text Analysis 
This notebook recreates Andrey Markov’s classic experiment on **vowel/consonant dependence** in Alexander Pushkin’s *Eugene Onegin*. It maps letters to two states - **V** (vowel) and **C** (consonant) - and tests whether successive letters are independent or exhibit Markovian dependence.

- An example of some Russian text. You can change it to other languages or even try it out on other data - any data where you can define a small set of "states" and observe sequences over time, you can do a transition-matrix analysis on. E.g. DNA and RNA bases, protein structures, client churn analysis, finanical volatility regimes, credit rating analysis, sports, and so on. 
- You can also try to perform an **independence check** using the chi-square test on adjacent pairs.
- Using the transition matrix you can also try to **simulate** a V/C sequence from the fitted chain, and create "new text" data.

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
