Humanoids 2020 Workshop: Talos: Status & Progress
=================================================

<img align="center" alt="Talos Family" src="talos_panel.png" style="max-width: 100%; margin: 1%;">

Organizers:
* Alexander Werner, University of Waterloo
* Olivier Stasse, LAAS-CNRS

# Workshop objectives
The goal of this workshop is to exchange information about control approaches for humanoid robots,  with the torque controlled robots such as the Talos platform in mind. Starting from a report on the experimentally discovered abilities of the hardware, further needed improvements will be discussed. To put this in context, speakers who work on other humanoid platforms have been invited. The objective here is to describe and compare viable ways to improve dynamic capabilities of this robot. Building on this discourse about structure and actuators, talks about whole body control control solutions are presented. Again, an open discussion in this workshop about particular topic will help the community to compare approaches and their properties. To complete the picture of progress on the Talos platform, talks about integrated contact planning and teleoperation are on the agenda. There are now 6 Talos robots in the world (PAL, LAAS, IJS, Waterloo, INRIA, Edinburgh) and this workshop will initiate further collaboration.


# Agenda

Note: The workshop core time is `13:30-13:45` - see [here](https://humanoids-2020.org/conference-program/index.html).

| Time         | Presenter                       | Talk Title                                   |
|--------------|---------------------------------|----------------------------------------------|
|08:00 - 08:30 | [Olivier Stasse](#stasse)       | SLAM and motion generation for Talos torque controlled robot |
|08:30 - 09:00 | [Steve Tonneau](#steve)         | Interactive multi contact planning algorithms for Talos |
|09:00 - 09:30 | [Adria Roig](#adria)            | Talos software stack upgrades and progress on whole body control |
|09:30 - 10:00 | [Vladimir Ivan](#vladimir)      | Talos use case: Planning jumping motion using direct transcription |
|--------------|---------------------------------|----------------------------------------------|
|10:00 - 10:30 |Coffee break                     |                                              |
|--------------|---------------------------------|----------------------------------------------|
|10:30 - 11:00 | [Jean-Baptiste Mouret and Serena Ivaldi](#jean) | Whole-body teleoperation and online, data-efficient learning of bad configurationsTalk #4 |
|11:30 - 12:00 | [Tadej Petric](#tadej) | Humanoids and physical human-robot interaction - learning by switching roles |
|12:00 - 12:30 | [Alexander Werner](#alexander) | Improving joint torque control performance and effects on whole body control |
|--------------|---------------------------------|----------------------------------------------|
|12:30 - 13:30 | Lunch break                 
|--------------|---------------------------------|----------------------------------------------|
|13:30         | Lightning talk #1
|13:35         | Lightning talk #2
|13:40         | Lightning talk #3
|13:45         | Q&A / Coffee & Snacks
|
|13:55         | Lightning talk #4
|14:00         | Lightning talk #5
|14:05         | Lightning talk #6
|14:10         | Q&A / Coffee & Snacks |
|
|14:20         | Lightning talk #7
|14:25         | Lightning talk #8
|14:30         | Lightning talk #9
|14:40         | Q&A / Coffee & Snacks |
|
|14:50         | Lightning talk #10
|14:55         | Lightning talk #11
|15:00         | Q&A / Coffee & Snacks |
|
|15:15 - 15:45 | Panel discussion | Technical readiness of human-scale Humanoids
|
|16:00 - 16:30 | [Jemin Hwangbo](#jemin) | TBA |
|16:30 - 17:00 | [Nikolaos Tsagarakis](#nikolaos) | Torque Control Actuation for Humanoid Robotics |
|17:00 - 17:30 | [Enrico Mingo](#enrico) | TBA |
|
|17:30 - 18:00 | Coffee break |
|
|18:00 - 18:30: | [Danielle Pucci](#danielle) | TBA |


## <a name="stasse"></a> Olivier Stasse (LAAS-CNRS): SLAM and motion generation for Talos torque controlled robot
<img align="left" alt="Olivier Stasse" src="olivier.jpeg" style="max-width: 25%; margin: 2%;">
TBA</br>


## <a name="steve"></a> Steve Tonneau (University of Edinburgh): Interactive multi contact planning algorithms for Talos
<img align="left" alt="Steve Tonnau" src="steve.png" style="max-width: 25%; margin: 2%;">
TBA</br>


## <a name="adria"></a> Adrià Roig (PAL Robotics): Talos software stack upgrades and progress on whole body control
<img align="left" alt="Adria Roig" src="adria.jpeg" style="max-width: 25%; margin: 2%;">
TALOS is a humanoid robot, designed in 2017 by PAL Robotics, that is present in many universities nowadays. This robot has been designed with the objective to perform industrial applications in the Factory of the Futures, as well as to interact in a real human environment. For this purpose, it is equipped with torque sensors in all joints, which enables powerful sensing and multi-contact motions. The closed-loop torque control can be used for whole-body control inverse dynamics and safe interaction with the environment. The motors of this robot can carry out fast movements and handle weights of 6 kg with an outstretched arm. The Ethercat communication allows running ROS control at 2KHz making it the perfect platform for researchers. In this presentation, we will present some of the latest developments of this platform which include WB-MPC and walking in uneven terrain.
</br>


## <a name="vladimir"></a> Vladimir Ivan (University of Edinburgh): Talos use case: Planning jumping motion using direct transcription
<img align="left" alt="Vladimir Ivan" src="vladimir.webp" style="max-width: 25%; margin: 2%;">
In this session we’ll report on the motion planning work that enabled us to execute jumping motion on the Talos robot. To achieve this, we formulated the problem using direct transcription as a sparse non-linear programming problem. We exploited the rigid body dynamics model of the robot and modelled the dynamic defect constraints using inverse dynamics as opposed to deriving the constraint from forward dynamics equations. The planned trajectories consist of feed forward torque and robot state reference trajectories. We implemented a torque controller that tracks the robot state with PD feedback and inputs the reference torque as a feed forward signal. This enabled us to execute the first jumping motion achieved on the Talos robot.
</br>

## <a name="jean"></a> Jean-Baptiste Mouret and Serena Ivaldi (INRIA): Whole-body teleoperation and online, data-efficient learning of bad configurations
<img align="left" alt="Jean-Baptiste Mouret" src="jean.jpg" style="max-width: 12%; margin: 2%;">
<img align="left" alt="Serena Ivaldi" src="serena.jpeg" style="max-width: 12%; margin: 2%;">
Abstract TBA
</br>

## <a name="tadej"></a> Tadej Petric (IJS): Humanoids and physical human-robot interaction - learning by switching roles
<img align="left" alt="Tadej Petrič" src="tadej.jpg" style="max-width: 25%; margin: 2%;">
Humanoid robots still have the shortcoming of limited ability to observe and adapt to human dynamics in physical human-robot collaboration. This leads to inefficient collaboration, skill transfer, and learning. In this talk, I will present how skill transfer can be achieved by switching the roles of the assistant agent and the assisted agent. Introducing such a strategy into the concept of learning from demonstrations (LfD) accelerates the learning process by providing a richer set of demonstrations with personalization capabilities. By including human-human, human-robot, and robot-human behaviors, we can gather a wider range of sensory information including force and motion trajectories. As an encoding strategy, we consider a novel holistic approach to encode the behavior of the two agents in a joint model that is used within regression and model predictive control strategies for reaction and anticipation of the agent behaviors.
</br>

## <a name="alexander"></a> Alexander Werner (University of Waterloo): Improving joint torque control performance and effects on whole body control
<img align="left" alt="Alexander Werner" src="alexander.png" style="max-width: 25%; margin: 2%;">
Abstract TBA
</br>

## <a name="jemin"></a>  Jemin Hwangbo (KAIST): TBA
<img align="left" alt="Jemin Hwangbo" src="jemin.webp" style="max-width: 25%; margin: 2%;">
Abstract TBA
</br>

##  <a name="nikolaos"></a> Nikolaos Tsagarakis (IIT): Torque Control Actuation for Humanoid Robotics
<img align="left" alt="Nikolaos Tsagarakis" src="nikolaos.jpeg" style="max-width: 25%; margin: 2%;">
Abstract TBA
</br>

##  <a name="enrico"></a> Enrico Mingo (IIT): TBA


##  <a name="danielle"></a> Daniele Pucci (IIT): TBA



