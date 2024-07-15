# Automated-Planning-Under-Interacting-Sources-of-Uncertainty

## Abstract


## Dependencies 
This project tackles the challenge of task planning under conditions of uncertainty, with a specific focus on managing temporal availability constraints. These constraints involve necessary resources being available only during limited time windows. To address this, we present an approach leveraging genetic algorithms to enhance both robustness and efficiency in smart Cyber-Physical Systems (sCPS) scenarios, such as electric vehicle charging and healthcare robotics.

Two specific strategies are employed to address the problem. The first strategy utilizes linear programming techniques with constraints, specifically the MILP (Mixed-Integer Linear Programming) algorithm. This approach does not consider uncertainty. The results from the MILP algorithm will serve as a baseline for comparison in terms of quality, effectiveness, and efficiency against the results achieved by the second strategy, which employs a multi-objective genetic algorithm that does take uncertainty into account.

The project is implemented in the latest version of Python (3.12.1) and requires the installation of the following libraries for its development and execution:

* Pulp 2.7.0
* NumPy 1.26.2
* Matplotlib 3.8.2
  
## Repository structure
This repository contains the following items:
* `Readme.md`: this file explaning the code of the project
* `Vehicles_algorithms`: this folder contains two files
  * `vehicles_without_uncertainty.ypinb`: this file contains the differente versions of the algorithms that solve the vehicle charging planning problem without considering uncertainty. This is where the implementation of the MILP algorithm used as the basis for the experiments is located.
  * `vehicles_under_uncertainty.ypinb`: this file contains the differente the algorithms that solve the vehicle charging planning problem considering uncertainty. This is where the implementation of the genetic algorithm used in experiments is located.
* `Robots_algorithms`: this folder contains the file `Robots_algorithms.ypinb`. In this file, we can find the two algorithms implemented to solve the problem of robots in the healthcare domain (The MILP algorithm that does not consider uncertainty and the genetic algorithm that does).
* * `Data`: in this folder we can find the data files used to run the experiments.
  * `example_vehicle_objects.txt`: code that contains the data you can modify and add to the algoritms code to conduct experiments. You can copy and paste all the content or part of it directly in the code.
  * `vehicles.txt` and `patients.txt`: data files used to run the algorithms in some experiments. These are files external to the code.
  * `evaluation_charts.ypinb`: code used to generate the evaluation charts included in the paper.
