## Introduction
### DATASET
"Pendulum Environment" from Open AI Gym library
- **Description** : The inverted pendulum swingup problem is based on the classic problem in control theory. The system consists of a pendulum attached at one end to a fixed point, and the other end being free. The pendulum starts in a random position and the goal is to apply torque on the free end to swing it into an upright position, with its center of gravity right above the fixed point. The diagram below specifies the coordinate system used for the implementation of the pendulum’s dynamic equations
  - x-y: cartesian coordinates of the pendulum’s end in meters.
  - theta : angle in radians.
  - tau: torque in N m. Defined as positive counter-clockwise. 
- **Action Space** : The action is a ndarray with shape (1,) representing the torque applied to free end of the pendulum
![image](https://user-images.githubusercontent.com/104628789/171803080-9cf417d2-8ef6-48af-8800-6f1f9e5a40d7.png)
- **Observation Space** : The observation is a ndarray with shape (3,) representing the x-y coordinates of the pendulum’s free end and its angular velocity.

![image](https://user-images.githubusercontent.com/104628789/171803147-fdc78f93-aaf1-4f40-8fb9-b51c6cd85232.png)
- **Reward** : The reward function is defined as:
r = -(theta2 + 0.1 * theta_dt2 + 0.001 * torque2)
where $    heta$ is the pendulum’s angle normalized between [-pi, pi] (with 0 being in the upright position). Based on the above equation, the minimum reward that can be obtained is -(pi2 + 0.1 * 82 + 0.001 * 22) = -16.2736044, while the maximum reward is zero (pendulum is upright with zero velocity and no torque applied).
## Model Training:
- Proximal Policy Optimization (PPO)
- Advantage Actor Critic (A2C)
- Deep Deterministic Policy Gradient (DDPG)
- Soft Actor-Critic (SAC)
- Twin Delayed Deep Deterministic Policy Gradient (TD3)

## Results
### Pre-and post training by algorithm
![image](https://user-images.githubusercontent.com/104628789/171804265-58aab0d9-1a7a-4cac-852c-a98b8abf92ae.png)

- **Observation**
In pendulum problem, PPO and A2C is not a suitable for this problem because it is not different between pre and post train.

### all algorithm
![image](https://user-images.githubusercontent.com/104628789/171804367-2995ff6b-2406-4baa-839d-dda8b50a36c7.png)

![image](https://user-images.githubusercontent.com/104628789/171804138-294192d5-ecd6-4b90-a430-088254d8c32b.png)
 it is unable to differentiate between "TD3, SAC and DDPG with post-training up to 1000 episode". Howevere, the winner of the pendulum problem is "DDPG".

## Notebook
you can find notebook [here](https://github.com/WarintornNawong/Portfolio/blob/main/Beat%20Pendulum%20gameplay%20with%20RL%20algorithm/Pendulum.ipynb)



