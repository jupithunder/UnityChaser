# UnityChaser
Multi-agent Reinforcement Learning Environment

A Unity ML-Agents based simulation environment that considers situations where multiple agents may have a common or conflicting purpose in the environment

<a href="https://github.com/Unity-Technologies/ml-agents">Unity ML-Agents</a>

## Documentation
<ul>
  The name of this simulation environment is Chaser, which is an environment that takes into account the situation where 1~N red balls follow 1~N blue balls in MxM size map.
  The blue ball disappears as soon as it hits the red ball. The game progresses until all blue balls disappear.
  

## State
<li>
Visual Observations
</li>
    Continuous image data from a camera attached to the ball
  
<li>
Vector Observations
</li>
    The vector distance difference between the 3D positions of the obstacles and different colored balls that are less than a certain distance within the viewing angle of the ball from the 3D position of the ball
  
  
  
## Action
<li>
Continuous action space
</li>
<li>
An action is represented by [x_torque, y_torque]
</li>
    One torque on each of the x and z axes into the [-1, 1] range


## Reward
<li>
Red Ball's Reward
</li>
    If it catches the blue ball, it gains +1 reward.
    It gains a reward of -0.001 every step.
    
<li>
Blue Ball's Reward - Preparing...
</li>
    If it disappears by a red ball, it gains -1 reward.
    It gains a reward of +0.001 every step.
    
</ul>

