# Using Deep Learning to Predict Human Decisions, and Cognitive Models to Explain Deep Learning Models
By Matan Fintz, Margarita Osadchy , Uri Hertz

[link to the paper] https://www.biorxiv.org/content/10.1101/2021.01.13.426629v2
## 1. About
This repo will allow the user to replicate the main experiments in the paper

### 2. Currently updated jupyter notebooks
  1. *Simulation_Comparisons*  
This notebook loads the results of simulation with the exploartory, reward oriented and reward oblivious models. Once the simulation results are loaded, the user can choose a distance function of choice for an aggregated comparison plots between the models. 
`produce_comparison_df()` takes a `dist_func` argument which can be any distance function that can take 2 vectors and return a distance (in our case, 2 arrays of size 4, as we have 4 sofmax values per prediction). In this notebook the distance metric, for example, is the symmetric KL distance.

More will be added soon.
