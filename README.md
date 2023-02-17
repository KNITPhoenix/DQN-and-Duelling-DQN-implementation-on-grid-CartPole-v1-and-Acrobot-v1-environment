# DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment

## Environments Description:
- Grid Environment : A 5X5 grid enironment, with 1 agent, 1 reward, 2 penalties and goal reward. The agent starts from (0,0) and the goal is set to (4,4). The possible actions can be {0:Right, 1:left, 2:Down, 3:Up}.
![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/grid.PNG)
- CartPole-v1 Environment : A pole is attached by an un-actuated joint to a cart, which moves along a frictionless track. The pendulum is placed upright on the cart and the goal is to balance the pole by applying forces in the left and right direction on the cart. Possible actions for environment are `{0, 1}`. The action is indicating the direction of the fixed force the cart is pushed with. It is { 0: Push cart to the left, 1: Push cart to the right }.
![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/cartpole.PNG)
- Acrobot-v1 Environment: Its an openAI gym environment, where system consists of two links connected linearly to form a chain, with one end of the chain fixed. The joint between the two links is actuated. The goal is to apply torques on the actuated joint to swing the free end of the linear chain above a given height while starting from the initial state of hanging downwards. Possible Actions are: {apply -1 torque to the actuated joint, apply 0 torque to the actuated joint, apply 1 torque to the actuated joint}. Possible states: The state is an 6-dimensional vector: {Cosine of ‘theta1’, Sine of ‘theta1’, Cosine of ‘theta2’, Sine of ‘theta2’, Angular Velocity of ‘theta1’, Angular Velocity of ‘theta2’}.

![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/acrobot.PNG)

## Algorithms
- DQN : Deep Q-Network, approximates a state-value function in a Q-Learning framework with a neural network. In the Atari Games case, they take in several frames of the game as an input and output state values for each action as an output.
- Duelling DQN : A Dueling Network is a type of Q-Network that has two streams to separately estimate (scalar) state-value and the advantages for each action. Both streams share a common convolutional feature learning module. The two streams are combined via a special aggregating layer to produce an estimate of the state-action value function Q .

## Results
- Grid: The reward per episode is calculated as the mean of all the rewards per episode. The network was trained for 1000 episodes with a discount factor of 0.93 (DQN) and 0.99 (Duelling DQN). It resulted in a reward of 240 (during testing).
- CartPole: The reward per episode is calculated as the mean of all the rewards per episode. We ran the network for 1000 episodes with a discount factor of 1. It resulted in a reward of 500 during testing.
- Acrobot: We ran the network for 1000 episodes with a discount factor of 0.93 (both) and got a reward of -100 during testing.
