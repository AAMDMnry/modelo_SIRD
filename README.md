# COVID-19 SIRD Modeling in Nuevo León

## Overview

This project analyzes COVID-19 data from Nuevo León, Mexico, and applies the SIRD epidemiological model to simulate the spread of the disease.

The objective is to compare real pandemic data with a mathematical model fitted through numerical optimization, allowing the study of infection, recovery, and mortality dynamics.

---

## Objectives

* Process and clean COVID-19 open data.
* Extract confirmed cases and deaths for Nuevo León.
* Implement the SIRD epidemiological model.
* Solve the differential equation system using the Runge-Kutta 4th Order method.
* Estimate model parameters from real data.
* Compare simulated and observed pandemic behavior.

---

## Dataset

The project uses COVID-19 open data records provided by Mexican health authorities.

### Data Processing

* Selection of confirmed COVID-19 cases.
* Filtering of records corresponding to Nuevo León.
* Conversion of date variables to datetime format.
* Construction of daily time series for:

  * New cases
  * Deaths
  * Active infections
  * Recovered individuals

---

## Mathematical Model

The SIRD model divides the population into four compartments:

* **S**: Susceptible individuals
* **I**: Infected individuals
* **R**: Recovered individuals
* **D**: Deceased individuals

The model is governed by a system of ordinary differential equations describing transitions between these populations over time.

### Parameters

* **β (beta)**: Infection rate
* **γ (gamma)**: Recovery rate
* **μ (mu)**: Mortality rate

---

## Numerical Methods

The differential equation system was solved using:

* Runge-Kutta Method (RK4)
* Numerical optimization with SciPy to estimate model parameters

The optimization process minimizes the difference between simulated and observed data.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Jupyter Notebook

---

## Results

The fitted model was used to generate:

* Daily infection curves
* Recovery curves
* Mortality curves
* Comparisons between real and simulated data

Visualizations allow evaluation of how well the SIRD model reproduces observed pandemic behavior.

---

## Repository Structure

```text
├── sird-model-nuevo-leon.ipynb
├── figures/
├── README.md
```

---

## Future Improvements

* Incorporate time-varying parameters.
* Evaluate alternative epidemiological models such as SEIR.
* Include vaccination effects.
* Compare different optimization strategies.
* Analyze additional Mexican states.

---

## Author

Angel Alejandro Monreal Durán

Mathematics Student | Data Science Enthusiast

