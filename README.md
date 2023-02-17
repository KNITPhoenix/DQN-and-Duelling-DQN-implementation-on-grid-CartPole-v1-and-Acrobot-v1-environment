# DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment

## Environments Description:
- Grid Environment : A 5X5 grid enironment, with 1 agent, 1 reward, 2 penalties and goal reward. The agent starts from (0,0) and the goal is set to (4,4). The possible actions can be {0:Right, 1:left, 2:Down, 3:Up}.
![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/grid.PNG)
- CartPole-v1 Environment : A pole is attached by an un-actuated joint to a cart, which moves along a frictionless track. The pendulum is placed upright on the cart and the goal is to balance the pole by applying forces in the left and right direction on the cart. Possible actions for environment are `{0, 1}`. The action is indicating the direction of the fixed force the cart is pushed with. It is { 0: Push cart to the left, 1: Push cart to the right }.
![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/cartpole.PNG)
- Acrobot-v1 Environment: Its an openAI gym environment, where system consists of two links connected linearly to form a chain, with one end of the chain fixed. The joint between the two links is actuated. The goal is to apply torques on the actuated joint to swing the free end of the linear chain above a given height while starting from the initial state of hanging downwards. Possible Actions are: {apply -1 torque to the actuated joint, apply 0 torque to the actuated joint, apply 1 torque to the actuated joint}. Possible states: The state is an 6-dimensional vector: {Cosine of ‘theta1’, Sine of ‘theta1’, Cosine of ‘theta2’, Sine of ‘theta2’, Angular Velocity of ‘theta1’, Angular Velocity of ‘theta2’}.

![alt text](https://github.com/KNITPhoenix/DQN-and-Duelling-DQN-implementation-on-grid-CartPole-v1-and-Lunar-Lander-environment/blob/main/acrobot.PNG)

