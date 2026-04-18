# Data Description

This folder contains the observed datasets used for parameter inference in the adaptive network epidemic model analysed in this project.

## Files

The following datasets are provided:

- **infected_timeseries.csv**

  Contains the infected-fraction time series for 40 independent simulation replicates observed over 201 time steps. These trajectories describe the evolution of the epidemic and are used to construct time-dependent summary statistics such as peak infected fraction, peak timing, and early growth rate.

- **rewiring_timeseries.csv**

  Contains the cumulative number of rewiring events recorded at each time step across the same 40 simulation replicates. These data provide information about behavioural adaptation in the network and are primarily informative about the rewiring parameter (ρ).

- **final_degree_histograms.csv**

  Contains the final degree distributions of the contact network at the end of each replicate simulation. These histograms capture structural changes in the network induced by rewiring dynamics and provide additional identification power for ρ.

## Usage

These datasets serve as fixed observational inputs for all Approximate Bayesian Computation (ABC) inference methods implemented in this repository:

- Basic Rejection ABC
- Regression Adjustment
- ABC-MCMC
- SMC-ABC
