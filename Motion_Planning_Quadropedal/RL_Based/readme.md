# RL Based Motion planning for Quadropedal Robots
***
## 2019

 ### [Learning to Walk via Deep Reinforcement Learning, 2019](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20Walk%20via%20Deep%20Reinforcement%20Learning.pdf)
The problem of sample efficiany is addressed via a noval approach to the maximal entropy Reinforcement learning replacing the manual tunning of the temperature (traditionally set namually for each task) with a constraint on the entropy and solving the constraint problem with a dual Lagrangian method. The approach is implemented on a small quadropedal robot which achives acceptable performance within 2 hour of training (~400 rollouts) with no pre-training in simulation.
***

### [Learning Agile and Dynamic Motor Skills for Legged Robots, 2019](/Motion_Planning_Quadropedal/RL_Based/Learning%20Agile%20and%20Dynamic%20Motor%20Skills%20for%20Legged%20Robots.pdf)

***

### [Robust Recovery Controller for a Quadrupedal Robot using Deep Reinforcement Learning, 2019](/Motion_Planning_Quadropedal/RL_Based/Robust%20Recovery%20Controller%20for%20a%20Quadrupedal%20Robot%20using%20Deep%20Reinforcement%20Learning.pdf)

***
## 2020

### [Learning Quadrupedal Locomotion over Challenging Terrain, 2020](/Motion_Planning_Quadropedal/RL_Based/Learning%20Quadrupedal%20Locomotion%20over%20Challenging%20Terrain.pdf)
This seminal paper is the brought to light the abbility to used RL method for complex motion planning tasks. The main result of this work is a highly robust controller for a quadropedal robot based solely on prioperceptive sensors capable of traversing extremly challenging terrains. It is this controller that wa used by cerberus team to win the DARPA subterenious challenge.
The main noval components are:
- **A novel teacher-student learning architectue** in which the teacher network learns both a latent space embedding and a policy via an RL method and the student learns the same elements (different architecture-TCN) learned with imitation learning in which the input to the embedding in a sequence of preoperceptive observations.
- **Curriculem learning**
- **Low level deployement of the policy**

![Teacher-Student](/Motion_Planning_Quadropedal/RL_Based/Teacher_student.png){:width="600px"}.


***

## 2021

### [Learning to jump from pixels, 2021](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20Jump%20from%20Pixels.pdf)

***

### [Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning, 2021](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20Walk%20in%20Minutes%20Using%20Massively%20Parallel%20Deep%20Reinforcement%20Learning.pdf)

***

### [RMA: Rapid Motor Adaptation for Legged Robots, 2021](/Motion_Planning_Quadropedal/RL_Based/RMA%20Rapid%20Motor%20Adaptation%20for%20Legged%20Robots.pdf)

![RMA Architecture](/Motion_Planning_Quadropedal/RL_Based/RMA.png){:width="600px"}.

This paper introduces the adaptation modual which may be seen as a system identification module for the enviroment physical parameters. The adaptation mudule learnes the latent enviromental factor encoding via supervised learning taking as an input a trajectory of robot states. 
Some key notions:
- The enviriment parameters include both terrain properties an robot parameters such as mass, C.O.M and Actuator parameters. 
- The base policy achived in the priveledge learning stage is the same as the one in the deployment, yet due to the fact that the adaptation learning is only exposed to good trajectories and so is the base policy, both are retrained (iteratevly) with online data untill convergence.
- The Adaptation mudule and the base policy are significantly different (in size and function) making the adaptation module not suited for high frequency inference, thus an asynchronous deployment is implemented.
- Training is completely performed in Simulation.



***

### [Walk These Ways, 2022](/Motion_Planning_Quadropedal/RL_Based/Walk%20These%20Ways.pdf)

***

## 2022

### [Legged Locomotion in Challenging Terrains using Egocentric Vision, 2022](/Motion_Planning_Quadropedal/RL_Based/Legged%20Locomotion%20in%20Challenging%20Terrains%20using%20Egocentric%20Vision.pdf)


***

### [Learning vision-guided quadrupedal locomotion end-to-end with cross-modal transformers, 2022](/Motion_Planning_Quadropedal/RL_Based/Learning%20Vision-Guided%20Quadrupedal%20Locomotion%20End-to-End%20with%20Cross-Modal%20Transformers.pdf)

***
### [Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion, 2022](/Motion_Planning_Quadropedal/RL_Based/Deep%20Whole-Body%20Control%20Learning%20a%20Unified%20Policy%20for%20Manipulation%20and%20Locomotion.pdf)

***

### [Adversarial Motion Priors Make Good Substitutes for Complex Reward Functions, 2022](/Motion_Planning_Quadropedal/RL_Based/Adversarial%20Motion%20Priors%20Make%20Good%20Substitutes%20for%20Complex%20Reward%20Functions.pdf)

***

### [DayDreamer: World Models for Physical Robot Learning, 2022](/Motion_Planning_Quadropedal/RL_Based/DayDreamer%20World%20Models%20for%20Physical%20Robot%20Learning.pdf)

***

### [Learning Visual Locomotion with Cross-Modal Supervision, 2022](/Motion_Planning_Quadropedal/RL_Based/Learning%20Visual%20Locomotion%20with%20Cross-Modal%20Supervision.pdf)

***

### [Learning robust perceptive locomotion for quadrupedal robots in the wild, 2022](/Motion_Planning_Quadropedal/RL_Based/Learning%20robust%20perceptive%20locomotion%20for%20quadrupedal.pdf)
[movie](https://www.youtube.com/watch?v=zXbb6KQ0xV8)

![Perceptive locomotion](/Motion_Planning_Quadropedal/RL_Based/Perceptive_locomotion.png){:width="700px"}.


## 2023

### [Robot Parkour Learning, 2023](/Motion_Planning_Quadropedal/RL_Based/Robot_Parkour_Learning.pdf)

***

### [Extreme Parkour with Legged Robots, 2023](/Motion_Planning_Quadropedal/RL_Based/Extreme%20Parkour%20with%20Legged%20Robots.pdf)
This work  applies the same principle of teacher-student framwork in order to enable extreem manuvers. The teacher is learned with sampeled hight map and in addition an "expert" direction for the manuver. 
The student policy, learned by imitaion, takes as an input both the robot state and an head facing depth camera and the output is the estimated expert direction and the latent enviroment estimation.
In addition the work presents a simple reward function structure, in particular for the jap jump.

***

### [Legs as Manipulator: Pushing Quadrupedal Agility Beyond Locomotion, 2023](/Motion_Planning_Quadropedal/RL_Based/Legs%20as%20Manipulator%20Pushing%20Quadrupedal%20Agility%20Beyond%20Locomotion.pdf)

***

### [Hybrid Internal Model: Learning agile legged locomotion with simulated robot responcse](/Motion_Planning_Quadropedal/RL_Based/HYBRID%20INTERNAL%20MODEL%20LEARNING%20AGILE%20LEGGED.pdf)

[Project page](https://junfeng-long.github.io/HIMLoco/)

The HIM (Hybrid Internal Model) motion control architecture takes insperation from the Internal Mode Control applied in classical control theory. The method adds an intrnal model of the system which outputs a latent next step estimation of the robot which is then fed into the policy to obtain the next action. 
The critic is exposed to priveledge knowledge (higth map and external forces) while the Internal Model (Source incoder) is exposed to a trajectory of Proprioceptive states.
The Internal nodel is trained with a form of contrastive learning.
In all this is a highly robust yet seems overly convoluded, in addition the current from does not include any etraproceptive observation (e.g., camera) however they may be easily integrated.
 
***

### [ANYmal Parkour: Learning Agile Navigation for Quadrupedal Robots, 2023](/Motion_Planning_Quadropedal/RL_Based/ANYmal%20Parkour:%20Learning%20Agile%20Navigation%20for%20Quadrupedal%20Robots.pdf)

***

### [DreamWaQ: Learning Robust Quadrupedal Locomotion With Implicit Terrain Imagination via Deep Reinforcement Learning, 2022](/Motion_Planning_Quadropedal/RL_Based/DreamWaQ:%20Learning%20Robust%20Quadrupedal%20Locomotion%20With%20Implicit%20Terrain%20Imagination%20via%20Deep%20Reinforcement%20Learning.pdf)

***

### [Adaptive Control Strategy for Quadruped Robots in Actuator Degradation Scenarios, 2023](/Motion_Planning_Quadropedal/RL_Based/Adaptive%20Control%20Strategy%20for%20Quadruped%20Robots%20in%20Actuator%20Degradation%20Scenarios.pdf)

## 2024

### [Agile Continuous jumping in Discontinuous Terrain, 2024](/Motion_Planning_Quadropedal/RL_Based/Agile%20Continuous%20Jumping%20in%20Discontinuous%20Terrains.pdf)

***

### [RL + Model-based Control: Using On-demand Optimal Control to Learn Versatile Legged Locomotion, 2024](/Motion_Planning_Quadropedal/RL_Based/RL%20+%20Model-based%20Control.pdf)


***

### [Stage-Wise Reward Shaping for Acrobatic Robots: A Constrained Multi-Objective Reinforcement Learning Approach, 2024](/Motion_Planning_Quadropedal/RL_Based/Stage-Wise%20Reward%20Shaping%20for%20Acrobatic%20Robots.pdf)

***

### [Deep Compliant Control for Legged Robots, 2024](/Motion_Planning_Quadropedal/RL_Based/Deep%20Compliant%20Control%20for%20Legged%20Robots.pdf)

This work represents a compliant control mechanism learned by a multistgae episoidc RL framework. Each episode contains three stages:
- Walking stage: Learn to walk undisturbed for 2 sec.
- Recovery stage: A disturbance is introduced to the simulation via velocity impulse input to the robot base, at this stage (for 1 sec) the reward for the base linear and angular velocity is replace with the avarage reward returned in the learning stage (No penalty).
- Post-recovery stage: the full reward term is returned making sure the robot resumes it course.

The resulting policy is shown to be not only more complient w.r.t. external disturbance but also better behaved when incountering dynamic obstacles and dealing with uneven/unstable terrain.

<font color='red'>
Lior: We could use the internal model approach and augment the reward structure to achive this complient behaviour.
</font>

***

### [Learning to Open and Traverse Doors with a Legged Manipulator, 2024](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20Open%20and%20Traverse%20Doors%20with%20Legged%20Manipulator.pdf)

***

### [Perceptive Pedipulation with Local Obstacle Avoidance, 2024](/Motion_Planning_Quadropedal/RL_Based/Perceptive%20Pedipulation%20with%20Local%20Obstacle%20Avoidance.pdf)

***

### [Learning Agile Locomotion on Risky Terrains, 2024](/Motion_Planning_Quadropedal/RL_Based/Learning%20Agile%20Locomotion%20on%20Risky%20Terrains.pdf)
 
 ***

 ### [Learning Risk-Aware Quadrupedal Locomotion using Distributional Reinforcement Learning, 2024](/Motion_Planning_Quadropedal/RL_Based/Learning%20Risk-Aware%20Quadrupedal%20Locomotion%20using%20Distributional%20Reinforcement%20Learning.pdf)

***

 ### [Learning to Adapt: Bio-Inspired Gait Strategies for Versatile Quadruped Locomotion](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20Adapt:%20Bio-Inspired%20Gait%20Strategies%20for%20Versatile%20Quadruped%20Locomotion.pdf)

This paper takes the RL approach to quadroped locomotion, realizing  the different motion gait are suitable to different terrain type and velocity two policies are designe.
The first is a locomotion policy which outputs the motion actions. The input to the locomotion policy is the velocity command concatenated with the policy selection, an integer [0,7].
The policy selection if the output if the policy selection policy which selects which gait parameters to apply. While the locomotion policy has a standart reward function the policy selection policy has an interesting structure as the parameters for the gait transition 
in the wild are not well defined, a primary discriminant is the CoT measure.
The paper makes use on additional structure such as a state estimator and and gate generator process which serves as a referance for the locomotion policy.
The work is done in RaiSim.
 ***

 ### [Robust Ladder Climbing with a Quadrupedal Robot, 2024](/Motion_Planning_Quadropedal/RL_Based/Robust%20Ladder%20Climbing%20with%20a%20Quadrupedal%20Robot.pdf)

 *** 

 ### [MBC: Multi-Brain Collaborative Control for Quadruped Robots, 2024](/Motion_Planning_Quadropedal/RL_Based/MBC:%20Multi-Brain%20Collaborative%20Control%20for%20Quadroped%20robots.pdf)

 ***

 ### [ Learning to Walk in confined spaces using 3D representation, 2024](/Motion_Planning_Quadropedal/RL_Based/Learning%20to%20walk%20in%20confined%20spaces%20using%203D%20representation,%202024.pdf)

 ***

 ### [DTC: Deep Tracking Control, 2024](/Motion_Planning_Quadropedal/RL_Based/DTC:%20Deep%20Tracking%20Control.pdf)

***

 ### [PA-LOCO: Learning Perturbation-Adaptive Locomotion for Quadruped Robots, 2024](/Motion_Planning_Quadropedal/RL_Based/PA-LOCO:%20Learning%20Perturbation-Adaptive%20Locomotion%20for%20Quadruped%20Robots.pdf)

 ***

 ### [Learning Visual Parkour from Generated Images , 2024](/Motion_Planning_Quadropedal/RL_Based/Learning%20Visual%20Parkour%20from%20Generated%20Images.pdf)

 ***

 ### [SoloParkour: Constrained Reinforcement Learning for Visual Locomotion from Privileged Experience, 2024](/Motion_Planning_Quadropedal/RL_Based/SoloParkour:%20Constrained%20Reinforcement%20Learning.pdf)

 ***

 ### [Adaptive Control Strategy for Quadruped Robots in Actuator Degradation Scenarios, 2024](/Motion_Planning_Quadropedal/RL_Based/Adaptive%20Control%20Strategy%20for%20Quadruped%20Robots%20in%20Actuator%20Degradation%20Scenarios.pdf)