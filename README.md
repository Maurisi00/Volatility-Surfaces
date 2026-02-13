# Implied Volatility & Volatility Surfaces

## Introduction

This **CUATS mini-project** focuses on computing the **Implied Volatility (IV)** of an option and plotting the **Volatility Surface**. We will also discuss how one can use volatility surfaces, or values derived from them, in trading strategies.

This document contains both **mathematical derivations** and **coding exercises** for you to complete as you read through (similar to the coding sessions ran during term).

> **Note on Difficulty:**
> The CUATS mini-projects are intended to be a **deeper dive** into a topic, so this will be longer and more involved than a typical coding session.
> * If you get stuck on the exercises (and can't progress even after looking at the hints), please **go to the GitHub page** for this project and ask for help.
> * Where possible, exercises are designed so you can skip one and still make progress. If you are waiting for a response on GitHub, try moving to the next section.

---

## Project Roadmap

The general structure of the project is as follows:

### 1. Imports and Libraries
* Setting up a virtual environment for the project.
* Overview of the Python libraries needed (NumPy, SciPy, Plotly, etc.).

### 2. What is the Volatility Surface?
* Black-Scholes call prices and the parameters involved.
* Definition of **Implied Volatility**: When does it exist?

### 3. Getting Options Chains Data
* How the `yfinance` library works to fetch live data.
* Creating a function to collate options chain information into a clean Pandas DataFrame.

### 4. Computing the Implied Volatility
* Analytical solution / estimates in special cases.
* **The Bisection Method**: A robust starting point.
* **The Newton-Raphson Method**: And its extensions.
* **Brent's Method**: The hybrid, efficient standard.

### 5. Interpolating and Plotting
* Importance of ensuring surfaces are **Arbitrage-Free**.
* Discussion of parametric models.
* **Linear Interpolation**.
* **Cubic Spline Interpolation (Clough-Tocher)**.
* Plotting the volatility surface in 3D.

### 6. Volatility Surface Terms and Properties
* Qualitative discussion of features: **Skew**, **Smiles**, and **Term Structure**.
* Typical shapes of these curves in different markets (Equity vs. FX vs. Commodities).

### 7. Extensions & Implementations
* Modifications and improvements to the project.
* Ideas for involved bonus extensions.
  
### 8. Trading Strategies
* Example implementations of how to use volatility surfaces directly in trading.
  
### 9. References.
