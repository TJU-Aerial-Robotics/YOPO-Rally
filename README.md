# YOPO-Rally
A Sim-to-Real Single-Stage Planner for Off-Road Terrain

> \[!NOTE]
>
> The code will be released soon.

## System Overview
![System Overview](.media/system-overview.svg)

## Simulator
Please refer to the [YOPO-Sim]().
![YOPO-Sim](.media/yopo-sim.jpg)

## Imitation Learning

### Cost Map Generation
The terrain is exported as the point cloud map, and is then processed by TTA (Terrain Type Analysis) to generate the cost map.

<!-- Video -->

### Data Acquisition
The depth image, position, and orientation of the vehicle are recorded in the simulator.

![Data Acquisition](.media/data-acquisition.jpg)

### Trajectory Optimization
Cone constraints are applied to each primitive anchor to confine the trajectory within the neural network’s output range.

<!-- Video -->

## Inference
The planner inputs depth image, velocity, goal vector, and outputs the candidate trajectories with the corresponding cost.

<!-- Video -->

## Experiments
Please refer to the [YOPO-Rally Video]() for the experiment results.