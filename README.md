# Navigation

This repository contains my **Deep Q Network** implementation on two environments in Pytorch.
* **Banana** - A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to: **0**-*move forward*, **1**-*move backward*, **2**-*turn left*, **3**-*turn right*.<br />
![alt text](https://github.com/vjrahil/Navigation/blob/master/Images/BananaEnvironment.jpeg)<br />
**Task:** *Train an agent to navigate a large world and collect yellow bananas, while avoiding blue bananas.*

* **LunarLander** - Landing pad is always at coordinates (0,0). Coordinates are the first two numbers in state vector. Reward for moving from the top of the screen to landing pad and zero speed is about 100..140 points. If lander moves away from landing pad it loses reward back. Episode finishes if the lander crashes or comes to rest, receiving additional -100 or +100 points. Each leg ground contact is +10. Firing main engine is -0.3 points each frame. Solved is 200 points. Landing outside landing pad is possible. Fuel is infinite, so an agent can learn to fly and then land on its first attempt. Four discrete actions available: do nothing, fire left orientation engine, fire main engine, fire right orientation engine.<br />
![alt text](https://github.com/vjrahil/Navigation/blob/master/Images/LunarLanderEnvironment.png)<br />
**Task:** *Train an agent to navigate in the space to learn how to land the spaceship perfectly on the landing pad.*

## File Details

* **Banana**
  * **Images** - *Result images.*
  * **Banana_DQN.ipynb** - *Deep Q Network implementation.*
  * **Banana_DDQN.ipynb** - *Double Deep Q Network implementation.*
  * **Banana_DDQN.ipynb** - *Duelling Network + Double Deep Q Network implementation.*
* **LunarLander**
  * **Images** - *Result images.*
  * **DQN.ipynb** - *Deep Q Network implementation.*
  * **DDQN.ipynb** - *Double Deep Q Network implementation.*
  * **DDDQN.ipynb** - *Duelling Network + Double Deep Q Network implementation.*
* **Images** - *Readme images.*

## Results
* **Banana**<br />
  * **DQN** -> ![DQN](https://github.com/vjrahil/Navigation/blob/master/Banana/Images/Banana_DQN.png)<br />
  * **DDQN** -> ![DDQN](https://github.com/vjrahil/Navigation/blob/master/Banana/Images/Banana_DDQN.png)<br />
  * **DDDQN** -> ![DDDQN](https://github.com/vjrahil/Navigation/blob/master/Banana/Images/Banana_DDDQN.png)<br />

* **LunarLander**<br />
  * **DQN** -> ![DQN](https://github.com/vjrahil/Navigation/blob/master/LunarLander/Images/LunarLander_DQN.png)<br />
  * **DDQN** -> ![DDQN](https://github.com/vjrahil/Navigation/blob/master/LunarLander/Images/LunarLander_DDQN.png)<br />
  * **DDDQN** -> ![DDDQN](https://github.com/vjrahil/Navigation/blob/master/LunarLander/Images/LunarLander_DDDQN.png)<br />

## Observation
*DDQN* is able to solve the both environment with the minimum number of episodes. Hyperparameter tuning may result in better performance of *DDDQN* compared to *DDQN*.

## Enhancement
In this project, I have implemented the original DQN with some of the advancement.

* **Double DQN** [Paper](https://arxiv.org/abs/1509.06461)
* **Duelling Network** [Paper](https://arxiv.org/abs/1511.06581)

There exist many other extensions that might improve the performance of *DQN*s

* **Prioritized Experience Replay(PER)** [Paper](https://arxiv.org/abs/1511.05952)
* **Distributional DQN** [Paper](https://arxiv.org/abs/1707.06887)
* **Noisy DQN** [Paper](https://arxiv.org/abs/1706.10295)

## Repository Instruction
  
  * Clone the directory by using this command.
```
    git clone https://github.com/vjrahil/Navigation
```
  * To install required dependencies via ```pip```.
```
    pip install -r requirements.txt
```


