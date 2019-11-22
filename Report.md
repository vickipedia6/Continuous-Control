# Banana Navigation

## Learning Algorithm

* The agent is trained using Deep Deterministic Policy Gradient algorithm.
* The sequence of the actor architecture is 
```
INPUT_SIZE = 33

```
```
A Fully Connected Layer with an input size of 33 and activation function tanh
```
```
A Fully Connected Layer with an input size of 128 and output size of 256 and an activation function tanh
```
```
A Fully Connected Layer with an input size of 256 and output size of 512 and an activation function tanh
```
```
A Fully Connected Layer with an input size of 512 and output size of 4 and an activation function tanh
```

* The initial weights are initialized in a uniform distribution

* The sequence of the critic architecture is
```
INPUT_SIZE = 4
```
```
A Fully Connected Layer with an input size of 4 and activation function Leaky Relu
```
```
A Fully Connected Layer with an input size of 256 and output size of 256 and an activation function Leaky Relu
```
```
A Fully Connected Layer with an input size of 256 and output size of 256 and an activation function Leaky Relu
```
```
A Fully Connected Layer with an input size of 256 and output size of 1
```

### Hyper parameters

BUFFER_SIZE = int(1e6)  
BATCH_SIZE = 256        
GAMMA = 0.99            
TAU = 1e-3              
LR_ACTOR = 1e-3 (Had to tweek this one to make the model converge faster)         
LR_CRITIC = 1e-3 (T
WEIGHT_DECAY = 0    

### Plot of Rewards

<img src="/plot.png" width=500 px />

* The agent was able to solve the environment in less than 200 episodes. Initially i tried with 3 FC Layers in Actor architecture but the model didn't converge. So i added another FC layer and tweek the hyperparameters and that did wonders. The agent was able to solve it quickly.

### Checkpoints

* Please load the pretrained model using the checkpoints 'actor.pth' and 'critic.pth'

### Future Ideas 

* I will definitely try to improve this using Proximal Policy Optimization, Asynchronous Actor Critic
