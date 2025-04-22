# Light Intensity Control Simulation (P/PI/PID Controller)

This project simulates a light intensity control system using **P**, **PI**, and **PID controllers**. The goal is to demonstrate how feedback control systems can be applied to regulate light intensity in an environment using interactive sliders to adjust the controller's parameters. This allows the user to experiment with different control strategies and observe their effect on the system's performance over time.

## Project Overview

In this project, I built a **simulation** where you can control the light intensity using various controllers (P, PI, and PID). The system simulates how the light changes over time by applying a control signal to adjust its intensity based on the error (difference between the desired intensity and actual intensity).

### How it Works:
1. **Proportional (P) Control:** The controller adjusts the light intensity proportionally to the error. The larger the error, the stronger the control signal.
2. **Proportional-Integral (PI) Control:** Adds an integral term to the proportional control to account for accumulated error over time, improving the long-term control.
3. **Proportional-Integral-Derivative (PID) Control:** Adds a derivative term that anticipates the future error, providing faster responses to changes in the error.

### Key Features:
- **Interactive Dashboard**: The project uses **ipywidgets** to create sliders for tuning the controller parameters (Kp, Ki, Kd) and setting the target light intensity.
- **Real-time Simulation**: The light intensity, error, and control signal are plotted over time, allowing the user to visualize the effect of different controller types.
- **Saving Parameters**: The best parameters used in the simulation (controller type, Kp, Ki, Kd, and target) can be saved into a JSON file for future use.
- **Interactive Experience**: This allows you to switch between different control modes (P, PI, PID) and observe how they affect the light intensity control.

## Technologies Used:
- **Python**: The project is implemented using Python, a versatile language for simulation and control systems.
- **Matplotlib**: Used for plotting real-time graphs of light intensity, error, and control signal.
- **Numpy**: Utilized for mathematical calculations like error computation and control signal update.
- **ipywidgets**: Provides interactive widgets (sliders, buttons) for adjusting parameters in real-time.
- **JSON**: For saving and loading the best parameters used in the simulation.

## Installation

To run this project, you need to have Python installed along with the required libraries. You can install them using the following command:

```bash
pip install matplotlib numpy ipywidgets
