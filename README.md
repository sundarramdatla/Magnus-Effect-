# 3D Sports Ball Trajectory Simulation

## Project Overview

Developed a MATLAB-based numerical simulation to model the three-dimensional motion of a spinning sports ball, incorporating aerodynamic drag, the Magnus effect, gravitational forces, ground friction, and repeated collisions. The project investigates how spin, aerodynamic forces, and surface interactions influence ball trajectories and bounce dynamics.

## Theory

The model applies Newton's second law to a system of coupled ordinary differential equations (ODEs), incorporating gravity, quadratic aerodynamic drag, and the Magnus effect.

Aerodynamic drag is modeled as:

$$\mathbf{F}_d=-\frac12\rho C_d A|\mathbf{v}|\mathbf{v}$$

The Magnus effect, which describes the aerodynamic force associated with ball rotation, is approximated using:

$$\mathbf{F}_M=C(\boldsymbol{\omega}\times\mathbf{F}_d)$$

Ground collisions are modeled using the coefficient of restitution, while surface friction and rotational dynamics are represented through Coulomb friction and the inertia tensor.

## How It Was Built

Developed a MATLAB numerical solver using the adaptive Runge–Kutta `ode45` method to integrate six coupled first-order ODEs governing three-dimensional position and velocity. Implemented nonlinear aerodynamic drag, spin-dependent Magnus forces, and gravitational acceleration to simulate ball trajectories. Developed an event-driven collision algorithm to detect ground contact, apply restitution-based vertical velocity updates, and model horizontal friction through additional ODE integration. Calculated collision-induced torque using cross products and updated angular velocity through rigid-body rotational dynamics, iterating across 10 successive collisions. Visualized results using three-dimensional trajectory animations, vertical displacement plots, and top-down motion analysis.

## Results

Simulated three-dimensional ball trajectories across 10 successive ground collisions, capturing the effects of aerodynamic drag, rotational forces, friction, and energy loss during rebounds. Generated numerical solutions and trajectory visualizations demonstrating how spin-dependent forces and collision dynamics influence horizontal displacement, vertical motion, and successive bounce behavior.

## Technologies

MATLAB, Numerical ODE Solvers, Adaptive Runge–Kutta Methods, Computational Mechanics, Nonlinear Dynamics, Rigid-Body Dynamics, Numerical Integration, Event Detection, 3D Data Visualization.
