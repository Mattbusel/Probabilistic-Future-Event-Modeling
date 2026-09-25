# Probabilistic Future Event Modeling

Forecasting that starts from possible futures and works backward to the best decision now.

> **Status: research proposal only.** This repository is a single README. There is no code, dataset or model yet; the phases below are a plan.

## The idea

Most forecasting models look at history and extrapolate forward. They struggle exactly when it matters most: black-swan events, geopolitical shocks and fast technology shifts that have no precedent in the training data.

This project proposes the reverse direction. Begin with a set of assumed future conditions, attach probabilities to them, and reason backward to the present decisions that hold up best across those futures. As new data arrives, the probabilities update and the recommended decisions change with them. The output is a probabilistic tree of future states rather than a single point forecast.

The approach is related to established work in scenario planning, backcasting and robust decision-making, combined with standard ML tools.

## Planned methods

- **Bayesian inference** to maintain and update probability distributions over future outcomes
- **Counterfactual reasoning** to compare alternative futures that follow from different assumptions
- **Markov decision processes** to define probabilistic transitions between future states
- **Reinforcement learning** to choose present actions that perform well across the modelled futures

## Plan

1. Define a data structure for scenarios that carries probabilistic constraints.
2. Build a Bayesian network that simulates future scenarios.
3. Add an RL agent that optimizes decision paths against those scenarios.
4. Train on real-world data (financial markets, global events, sports outcomes).
5. Validate by back-testing against historical counterfactuals and comparing with standard forecasting baselines.

A practical first step would be a small prototype in Python using a probabilistic programming library such as PyMC or pgmpy on a toy domain.

## Possible applications

- **Finance:** strategies that react to distributions over future prices rather than historical patterns alone
- **Strategic planning:** scenario planning for businesses and governments
- **AI policy:** decision frameworks that account for anticipated technical and regulatory shifts

## Get involved

Looking for people with backgrounds in ML, statistics, decision theory and game theory, and for suggestions of open datasets to test against. Open an issue or a pull request.
