# risk-appetite-Monte-Carlo
A Python-based financial simulation tool designed to model revenue and OIBDA uncertainty. This project moves beyond simple triangular distributions by implementing the Beta-PERT methodology for more accurate risk appetite assessment
This repository contains a robust Python implementation of a Monte Carlo Simulation designed for financial forecasting and risk appetite assessment. Unlike simplified models, this tool utilizes the Beta-PERT distribution, providing a more nuanced and realistic estimation of business risks by emphasizing the "most likely" scenarios while accounting for tail-end uncertainties.
Key Features

    Probabilistic Revenue Modeling: Simulates multiple revenue streams using custom risk coefficients.

    Beta-PERT Implementation: Leverages scipy.stats.beta to model expert estimates (Min, Mode, Max) with higher statistical accuracy than standard triangular distributions.

    Risk Appetite Analysis: Calculates Value at Risk (VaR) and provides a cumulative distribution function (ECDF) to support data-driven decision-making.

    Comprehensive Visualization: Includes distribution histograms and probability density plots using seaborn and matplotlib.

Why PERT?

In financial risk management, the PERT distribution is preferred over the Triangular distribution because it smooths the probability curve and reduces the overweighting of extreme outliers. This results in a more reliable mean and standard deviation for EBITDA and Gross Profit forecasts.
Technical Stack

    Python 3.12+

    Libraries: numpy, pandas, scipy, matplotlib, seaborn

Usage

    Define your financial items in the REVENUE_ITEMS and EXPENSE_ITEMS dictionaries.

    Run the simulation (default: 10,000 iterations).

    Analyze the generated charts to determine the probability of meeting target KPIs.
