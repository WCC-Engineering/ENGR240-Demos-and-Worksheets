# Project 3: Vehicle Suspension Analysis

## Objectives
- Determine the appropriate method to integrate a set of experimental data
- Determine the appropriate method to differentiate a set of experimental data
- Develop effective figures for communicating results

## Problem Statement
The data file `project3_accel.dat` contains simulated acceleration data from a performance test on a vehicle suspension system. The data file includes time (in seconds) in the first column and vertical acceleration (in m/s²) of the vehicle center of mass in the second column. The data is estimated to have an uncertainty in the acceleration measurements of ± 0.5 m/s².

For this project, you will work with this data to determine the velocity, the position, and the jerk (the time derivative of acceleration), of the vehicle center of mass.

### Velocity and Position
You will need to integrate the data once to find velocity and again to find position:

$v(t) = v_0 + \int_{0}^{t} a(t) dt$ and $s(t) = s_0 + \int_{0}^{t} v(t) dt$

Take the initial velocity as $v_0 = -1.6$ m/s and the initial position to be $0$ m for these integrations. Consider the following integration approaches as you determine the most accurate and efficient approach to this problem:

- Integrating the data directly with composite trapezoid rule.
- Interpolating the data onto a finer interval and integrating the result with composite trapezoid rule.
- Assuming the system can be modelled as a damped oscillation and computing the coefficients for the least-squares curve fit of the mathematical model:
  $a(t) = Ae^{Bt} \cos(Ct + D)$
  to the data and integrating the result (numerically or analytically).

### Jerk
Determine and implement an accurate and efficient approach to differentiate this data to calculate the jerk:
$j(t) = \frac{da}{dt}$

Consider the following approaches to differentiating this data set:
- Applying appropriate finite difference formulas directly to the data.
- Interpolating the data onto a finer interval and differentiating the result with finite difference formulas.
- Assuming the system can be modelled as a damped oscillation and computing the coefficients for the least-squares curve fit of the mathematical model:
  $a(t) = Ae^{Bt} \cos(Ct + D)$
  to the data and differentiating the result (numerically or analytically).

## Instructions
Open the accompanying Python notebook in Google Colab to complete this project. The notebook contains starter code and guidance to help you solve the problem.

## Deliverables
Submit your completed Google Colab notebook with:
1. Working code implementing your solution
2. Results presented graphically in the notebook
3. Discussion section answering all the required questions

Be sure to review the grading rubric in Canvas to ensure you understand the project expectations.