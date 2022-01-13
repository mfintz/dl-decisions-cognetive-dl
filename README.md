# Using Deep Learning to Predict Human Decisions, and Cognitive Models to Explain Deep Learning Models
### By Matan Fintz *, Margarita Osadchy , Uri Hertz


[link to the paper](https://www.biorxiv.org/content/10.1101/2021.01.13.426629v2)
## 1. About
This repo will allow the user to replicate the main experiments in the paper

### 2. Currently updated jupyter notebooks
  1. *Simulation_Comparisons*  
This notebook loads the results of simulation with the exploartory, reward oriented and reward oblivious models. Once the simulation results are loaded, the user can choose a distance function of choice for an aggregated comparison plots between the models. 
`produce_comparison_df()` takes a `dist_func` argument which can be any distance function that can take 2 vectors and return a distance (in our case, 2 arrays of size 4, as we have 4 sofmax values per prediction). In this notebook the distance metric, for example, is the symmetric KL distance.
  2.  *preprocess*    
 The preprocessing of the raw data can be reproduced using this notebook, along with some exploration of the original data. This notebook is also used to create sequence is different sizes for later experiments.
  3. *Qlearning_model*
  This notebook contains the Qlearning model (Reward Oriented model) - from optimization steps (and task simulation for each participant using the optimized values) to recreating the plots. The plots are saved in svg format and later being edited.

More will be added soon.


* Part of Matan Fintz's Thesis

If using this repo or parts of it in any work, please provide a reference to:

```
@article {Fintz2021.01.13.426629,
	author = {Fintz, Matan and Osadchy, Margarita and Hertz, Uri},
	title = {Using Deep Learning to Predict Human Decisions and Cognitive Models to Explain Deep Learning Models},
	elocation-id = {2021.01.13.426629},
	year = {2021},
	doi = {10.1101/2021.01.13.426629},
	publisher = {Cold Spring Harbor Laboratory},
	abstract = {Deep neural networks (DNN) models have the potential to provide new insights in the study of human decision making, due to their high capacity and data-driven design. While these models may be able to go beyond theory-driven models in predicting human behaviour, their opaque nature limits their ability to explain how an operation is carried out. This explainability problem remains unresolved. Here we demonstrate the use of a DNN model as an exploratory tool to identify predictable and consistent human behaviour in value-based decision making beyond the scope of theory-driven models. We then propose using theory-driven models to characterise the operation of the DNN model. We trained a DNN model to predict human decisions in a four-armed bandit task. We found that this model was more accurate than a reinforcement-learning reward-oriented model geared towards choosing the most rewarding option. This disparity in accuracy was more pronounced during times when the expected reward from all options was similar, i.e., no unambiguous good option. To investigate this disparity, we introduced a reward-oblivious model, which was trained to predict human decisions without information about the rewards obtained from each option. This model captured decision-sequence patterns made by participants (e.g., a-b-c-d). In a series of experimental offline simulations of all models we found that the general model was in line with a reward-oriented model{\textquoteright}s predictions when one option was clearly better than the others. However, when options{\textquoteright} expected rewards were similar to each other, it was in-line with the reward-oblivious model{\textquoteright}s pattern completion predictions. These results indicate the contribution of predictable but task-irrelevant decision patterns to human decisions, especially when task-relevant choices are not immediately apparent. Importantly, we demonstrate how theory-driven cognitive models can be used to characterise the operation of DNNs, making them a useful explanatory tool in scientific investigation.Author Summary Deep neural networks (DNN) models are an extremely useful tool across multiple domains, and specifically for performing tasks that mimic and predict human behaviour. However, due to their opaque nature and high level of complexity, their ability to explain human behaviour is limited. Here we used DNN models to uncover hitherto overlooked aspects of human decision making, i.e., their reliance on predictable patterns for exploration. For this purpose, we trained a DNN model to predict human choices in a decision-making task. We then characterised this data-driven model using explicit, theory-driven cognitive models, in a set of offline experimental simulations. This relationship between explicit and data-driven approaches, where high-capacity models are used to explore beyond the scope of established models and theory-driven models are used to explain and characterise these new grounds, make DNN models a powerful scientific tool.Competing Interest StatementThe authors have declared no competing interest.},
	URL = {https://www.biorxiv.org/content/early/2021/01/15/2021.01.13.426629},
	eprint = {https://www.biorxiv.org/content/early/2021/01/15/2021.01.13.426629.full.pdf},
	journal = {bioRxiv}
}
```
