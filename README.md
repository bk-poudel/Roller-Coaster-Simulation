# Rollercoaster-Cart Simulation

## Overview
This project simulates the motion of a rollercoaster-cart on a track under the influence of gravity, friction, and air resistance. The simulation provides insights into the forces acting on the cart and evaluates the effectiveness of an initial thrust provided by a PMLSM (Permanent Magnet Linear Synchronous Motor). The model is flexible, allowing users to tweak environmental parameters and motor properties to test various scenarios.

The simulation utilizes MATLAB/Simulink, Python, and SolidWorks to model and analyze the system.

## Features
- **Physics-based Simulation**: Includes gravity, friction, and air resistance.
- **Customizable Parameters**: Users can adjust motor properties, environmental conditions, and track profiles.
- **Dynamic Motion Analysis**: Real-time feedback for velocity, acceleration, and position.
- **Forces Analysis**: Calculation of gravitational, frictional, and air resistance forces.
- **Multiple Track Profiles**: Supports sections with horizontal and inclined slopes.

## System Overview
The project consists of two main subsystems:

### 1. PMLSM Motor Subsystem
**Inputs:**
- Desired position behavior of the rollercoaster-cart.
- Motor parameters:
    - Fmax: Maximum thrust (e.g., 2000 N).
    - PM: Permanent magnet flux linkage (e.g., 0.65 Wb).
    - Ld, Lq: Inductance values (e.g., 0.01 H).
    - L0: Zero-sequence axis inductance (e.g., 2 × 10⁻⁴ H).
    - Rs: Stator resistance (e.g., 0.6 Ω).
    - Mass: Mass of the moving part (e.g., 1000 kg).
    - Pitch: Polar pitch (e.g., 0.1 m).
    - Np: Electrical pole-pair constant (e.g., π/Pitch rad/m).

**Output:**
- Thrust generated by the motor.

### 2. Rollercoaster Subsystem
**Inputs:**
- Track profile (length and slope variations).
- Environmental parameters:
    - Gravity
    - Friction
    - Air resistance
- Thrust from the motor.

**Outputs:**
- Motion analysis of the cart (acceleration, velocity, position).
- Force breakdown:
    - Gravitational force
    - Frictional force
    - Air resistance
- Evaluation of motor thrust adequacy.

## Relevance in Mechatronics and Robotics
Simulation software plays a critical role in engineering design, offering a cost-effective way to test and optimize systems before implementation. This project demonstrates the use of simulation tools to model a dynamic mechatronic system, analyze performance, and predict real-world behavior with minimal error.

## Prerequisites
- MATLAB/Simulink

## Installation
Clone this repository:
```bash
git clone https://github.com/bk-poudel/Roller-Coaster-Simulation.git
```

Open and configure the simulation files in MATLAB/Simulink as needed.

## Usage
1. Define the motor and environmental parameters in the `parameters.py` or Simulink model.
2. Set up the track profile in the provided scripts or SolidWorks model.
3. Run the simulations:
     - MATLAB/Simulink: Open and run `rollercoaster_sim.slx`.
4. Analyze outputs for acceleration, velocity, position, and force breakdowns.

## Outputs
The simulation provides:
-Animation of rollercoaster motion over the track
- Graphs for acceleration, velocity, and position over time.
- Force analysis (gravitational, frictional, air resistance).
- Feedback on motor thrust adequacy.

## Contributors
- Chengze Song
- Bibek Poudel

## License
This project is licensed under the MIT License.

## Feedback
For issues or suggestions, please create an issue or reach out via email bp2376@nyu.edu
