# A2C_demo


This repo is a place for me to demonstrate and compound my knowledge of the Actor critic algo.



Some RL algorithms will fall under a category of having high variance. In the RL space, the bias and variance dont just refer to how well the model fits training data, but also checks how well the RL model reflects the true reward structure of the environment. Variance refers to a noisy, but on average accurate value estimate, whereas bias refers to a stable, but inaccurate value estimate. What we mean by high variance is that the model learns the training set really well but fails to capture the generalizaiton of the data. High Bias refers to when a model is not able to get 



We use a combination of policy-based and value-based methods to reduce the variance,aka Actor-Critic method. The idea behind Actor-Critic method is that we learn two functions approximations. 
The actor: policy functions and the Critic: value function. The policy controls how our agent acts and the value functions assists in updating the policy by measuring how good the action is taken. The critic updates the value function parameters w and depending on the algorithm it could be a action-value Qw(a|s) or state-value Vw(s). Actor updates the policy parameters theta for pitheta(a|s), in the direction suggested by the critic. When specifically talking about A2C, we use the advantage function for our estimates instead of the action-value function. Advantage function calculates the relative advantage of an action compared to the other possible state i.e when this action is take at this state when compared to the average value of the state. It subtracts the mean value of the state from the state action pair. Advantage function requires two value functions Q(s,a) and V(s). We can use the TD error as a good estimator of the advantage function. 

