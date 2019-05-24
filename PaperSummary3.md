#A Deep Reinforcement Learning Driving Policy for Autonomous Road Vehicles 

This is a summary for the paper: [A Deep Reinforcement Learning Driving Policy for Autonomous Road Vehicles|https://arxiv.org/abs/1905.09046]


Problem: Driving policy for autonomous vehicles on highway

Why: 
Humans can easily follow a route suggested by the navigation system by effectively maneuvering the vehicle to avoid obstacles.
But, for an autonomous vehicle, it becomes necessary to guide the vehicles to follow the route suggested by the navigation. There needs to be a system that can make tactical maneuver decisions, for example, switch lanes, continue straight, etc.,  which can be translated to low level controls like steering wheel angle, speed etc. 

What:
The authors propose a Reinforcement learning model using DDQN to derive a driving policy for an autonomous vehicle on a highway.  The object function defined for the RL model also takes into account the comfort of passengers. 
The RL framework consists of a state space and an action space. A scalar reward r is assigned as a consequence of taking action a at a state s. The DDQN is trained based on a state representation that has information about absolute velocity of vehicle and relative positions of other vehicles. The action space consists of simple actions like changing lanes, accelerate/decelerate/ continue straight. The rewards signal is made up of penalties for collision, deviations from desired speed and unnecessary lane changes and accelerations.

