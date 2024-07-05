# Bayesian Analyses
Project of Advanced Statistical Modeling (ASM) Course for Master in Data Science Program of Universitat Politècnica de Catalunya (UPC)
***

This repository contains solutions to two Bayesian assignments focusing on different applications of Bayesian statistics. Each assignment is provided with a detailed analysis, including prior and posterior distributions, credible intervals, and other relevant calculations.

## Assignments Overview

### [Assignment 1](./docs/Traffic%20accidents%20statement.pdf): Traffic Accidents (Poisson)

#### Problem Statement

The weekly number of traffic accidents on La Garriga’s highway follows a Poisson(µ) distribution. Three students are counting the number of accidents for each of the next eight weeks. The data collected is as follows: 3, 2, 0, 8, 2, 4, 6, 1.

**Students' Prior Information:**
1. **Bru:** No prior information. Uses a Gamma(0.01, 0.001) prior for µ.
2. **Clàudia:** Lives in La Garriga. Uses a Gamma(6.25, 2.5) prior for µ.
3. **Carles:** Claims no prior information, uses an improper flat prior, π(µ)=1 for µ>0.

**Tasks:**
a) Draw the three prior distributions on the same graph.
b) Draw the likelihood function.
c) Draw the three posterior distributions on the same graph.
d) Calculate a 90% credible interval for the number of accidents for the next weekend for each Bayesian model.

### [Assignment 2](./docs/Yield%20potatoes%20statement.pdf): Yield of Potatoes

#### Problem Statement

A researcher is investigating the relationship between the yield of potatoes (y) and the level of fertilizer (x). The field is divided into eight plots, with different levels of fertilizer applied to each plot. The recorded data is as follows:

| Fertilizer Level (x) | Yield (y) |
|----------------------|-----------|
| 1                    | 25        |
| 1.5                  | 31        |
| 2                    | 27        |
| 2.5                  | 28        |
| 3                    | 36        |
| 3.5                  | 35        |
| 4                    | NA        |
| 4.5                  | 34        |

The yield given the fertilizer level is assumed to follow a `Normal(β0 + β1x, σ)` distribution.

**Tasks:**
a) Using non-informative priors for the parameters, draw the posterior distribution for all parameters.
b) Calculate a **95%** credible interval for each parameter.
c) Calculate a **95%** credible interval for y given `x = 4`.


### JAGS (Just Another Gibbs Sampler)

JAGS is used in `Assignment 2` for Bayesian inference. It is a program for the analysis of Bayesian hierarchical models using **Markov Chain Monte Carlo (MCMC)** simulation.

## Solution Files

### [traffic-accidents.html](./html/traffic-accidents.html)

The solution to `Assignment 1` includes:
- Graphs showing the prior distributions for Bru, Clàudia, and Carles.
- The likelihood function based on the collected data.
- Posterior distributions for each student's model.
- Calculations of the **90%** credible intervals for the number of accidents next weekend.

### [yield-potatoes.html](./html/yield-potatoes.html)

The solution to `Assignment 2` includes:
- Posterior distributions for the parameters **β0**, **β1**, and **σ**.
- **95%** credible intervals for the parameters.
- A **95%** credible interval for the yield `(y)` given the fertilizer level `(x) = 4`.

## Instructions for Viewing Solutions

To view the detailed solutions and graphical analyses, open the respective HTML files in a web browser:
- [Traffic Accidents Solution](./traffic-accidents.html)
- [Yield of Potatoes Solution](./yield-potatoes.html)
