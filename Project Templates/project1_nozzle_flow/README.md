# Project 1: Converging-Diverging Nozzle Flow Analysis

## Objectives
- Formulate and solve roots problems
- Determine the appropriate algorithm and numerical parameters for accuracy and efficiency
- Develop effective figures for communicating numerical results

## Problem Statement
Converging-diverging nozzles are required to accelerate a gas to velocities greater than the speed of sound. They are a standard component in aircraft and spacecraft propulsion systems.

For supersonic one-dimensional idealized gas flow (isentropic) in a converging-diverging nozzle, the relationship between the nozzle cross-sectional area, A, and the Mach number, M is given by:

$\frac{A}{A^*} = \frac{1}{M}\left[\left(\frac{2}{k+1}\right)\left(1+\frac{k-1}{2}M^2\right)\right]^{\frac{k+1}{2(k-1)}}$

Where A* is the area at the throat used to normalize A into the dimensionless area. The parameter k is the specific heat ratio for the gas. Two values of M exist for each value of the normalized area - one value less than 1 (subsonic flow) and one value greater than 1 (supersonic flow).

## Instructions
Open the accompanying Python notebook in Google Colab to complete this project. The notebook contains minimal starter code and a guide to help you solve the problem.

You are required to solve for both M results (subsonic and supersonic) for values of A/A* ranging from 1.1 to 10.0 (note that M = 1 when A/A* = 1) and for representative values of k including:
- k = 1.285 (CO₂)
- k = 1.400 (Air)
- k = 1.667 (noble gasses)

## Deliverables
Submit your completed Google Colab notebook with:
1. Working code implementing your solution
2. Results presented graphically in the notebook
3. Discussion section answering all the required questions

Be sure to review the grading rubric in Canvas to ensure you understand the project expectations.