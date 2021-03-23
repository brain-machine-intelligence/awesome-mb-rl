# Awesome Model-based RL Papers

**Awesome Model-based RL Papers**

# Table of Contents
+ [Papers](#papers)
  - [Surveys](#surveys)
  - [Dyanmics Model](#dynamics-model)
    - [Vae-based](#vae-based)
    - [Gan-based](#gan-based)
    - [Self-supervised](#self-supervised)
    - [Generalization](#generalization)
    - [Inductive bias](#inductive-bias)
  - [Planning](#planning)
    - [Shooting](#shooting)
    - [Population-based](#pop-based)
    - [CEM](#cem)
    - [Dyna-style](#dyna-style)
    - [MF-assisted](#mf-assisted)
    - [Local-to-global](#local-to-global)
    - [Estimate-derivative](#estimate-derivative)
+ [Lectures]($lectures)   
+ [Environments](#environment)
    

# Papers

## Surveys
+ 2019 | Benchmarking Model-based Reinforcement Learning | arXiv | [`PDF`](https://arxiv.org/abs/1907.02057)
  - keywords
    - Non-pixel-level, Extreme experiments
  - summary
    - (a) Tested a various model-based approaches on the unified test environment.

## Dyanmics Model
### Vae-based
+ 2019 | Learning Latent Dynamics for Planning from Pixels | ICML | [`PDF`](https://arxiv.org/abs/1811.04551) :star:
  - keywords
    - Pixel-level, VAE-based, CEM
  - summary
    - (a) Proposed a latent overshooting method that is more robust to n-step prediction. 
+ 2018 | World Models | arXiv | [`PDF`](http://arxiv.org/abs/1803.10122)
  - Pixel-level, VAE-based, Population-based
  - summary
    - (a) Proposed a VAE architecture that returns a next state and reward from the current state and action. 
    - (b) Learned dynamics model substitutes the real environment and interacts with the policy network (controller) to find the best policy. 

  
### Gan-based

### Self-supervised
+ 2020 | Goal-Aware Prediction: Learning to Model What Matters | ICML | [`PDF`](https://arxiv.org/abs/2007.07170)
  - keywords
    - Pixel-level, VAE-based, CEM
  - summary
    - (a) Proposed a self-supervised approach to guide the model better predicts a task relevant state information. 
    - (b) Using CEM, they sampled sub-optimal sequence which the last observation is considered as goal. (self-supverised)
    - (c) The model is trained to predict the pixel-level difference between the current observation and the goal's. (task-relevant feature)

### Generalization
+ 2020 | Context-aware Dynamics Model for Generalization in Model-Based Reinforcement Learning | ICML | [`PDF`](https://arxiv.org/pdf/2005.06800.pdf)
  - keywords
    - Non-pixel-level, Environment generalization
  - summary
    - (a) Proposed a dynamics-specific context encoder that captures contextual information and then predicts dynamics. 
    - (b) Learn a latent context vector from the local dynamics.
    - (c) Predicts the next state conditioned on context vector.

+ 2019 | Environment Probing Interaction Policies | ICLR | [`PDF`](https://arxiv.org/pdf/1907.11740.pdf)
  - keywords
    - None-pixel-level, Environment generalization
  - summary
    - (a) Proposed an environment probing policy that extracts implicit understanding of the environment.
    - (b) Learned environment-specific information is used when training a task-specific policy.
    - (c) Environment probing policy gets the positive reward in the case where the state prediction loss becomes smaller by adding
     environment-specific information.

### Inductive bias

## Planning

### Shooting

### CEM
tset
### Dyna-style

### MF-assisted
+ 2017 | MBMF: Model-Based Priors for Model-Free Reinforcement Learning | CoRL | [`PDF`](https://arxiv.org/abs/1709.03153)
  - keywords
    - Non-pixel-level, MF
  - summary
    - TODO
    
+ 2017 | Neural Network Dynamics for Model-Based Deep Reinforcement Learning with Model-Free Fine-Tuning | NeurIPS | [`PDF`](https://arxiv.org/abs/1708.02596)
  - keywords
    - Non-pixel-level, MF 
  - summary
    - TODO
    
### Estimate-derivative
