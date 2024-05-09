# A2C_demo


This repo is a place for me to demonstrate and compound my knowledge of the Actor critic algo.



Some RL algorithms will fall under a category of having high variance. In the case of RL, variance refers to a noisy, but on average accurate value estimate, whereas bias refers to a stable, but inaccurate value estimate. What we mean by high variance is that the model learns the training set really well but fails to capture the generalizaiton of the data. When the model fits really well.


We use a combination of policy-based and value-based methods to reduce the variance,aka Actor-Critic method. The idea behind Actor-Critic method is that we learn two functions approximations. 
The actor: policy functions and the Critic: value function. The policy controls how our agent acts and the value functions assists in updating the policy by measuring how good the action is taken. The critic updates the value function parameters w and depending on the algorithm it could be a action-value Qw(a|s) or state-value Vw(s). Actor updates the policy parameters theta for pitheta(a|s), in the direction suggested by the critic. 

The flow of actor-critic method

1) 
