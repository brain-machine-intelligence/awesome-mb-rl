# Awesome Model-based RL Papers
Awesome Model-based RL Papers

- Context-aware Dynamics Model for Generalization in Model-Based Reinforcement Learning
    - ICML 2020
    - UC Berkeley, KAIST
    - CaDM
    - https://arxiv.org/pdf/2005.06800.pdf
    - summary
        - Learn a global dynamics model that (a) learn a context latent vector that captures the local dynamics, then (b) predicting the next state conditioned on it
- Environment Probing Interaction Policies
    - ICLR 2019
    - Abhinav Gupta, CMU, Facebook AI Research
    - EPI
    - https://arxiv.org/pdf/1907.11740.pdf
    - summary
        - task-specific policy 와는 별개로 EPI (Environment Probing Interaction) Policy 를 통해 "environment-probing" trajectory 를 얻고, 그걸 이용해서 environment embedding 만들고, 그걸 task-specific policy 의 input 으로 사용 (transfer)
            - EPI policy 의 reward 는 next state transition prediction 을 environment embedding 없이 predict 하는 model 보다 더 잘 하는 정도 (diff)
            - epi prediction model 과 embedding network 동시 학습)