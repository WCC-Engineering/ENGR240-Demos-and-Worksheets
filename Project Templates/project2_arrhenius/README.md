# Project 2: Arrhenius Equation Curve Fitting

## Objectives
- Determine the appropriate curve-fitting algorithm to fit a model to a set of empirical data
- Interpret curve fit quality statistics
- Develop effective figures for communicating curve fitting results

## Problem Statement
The general form of the Arrhenius equation used to model the temperature dependence of the reaction rate for chemical reactions is:

$$k = A e^{-E/(RT_a)}$$

where k is the reaction rate (s⁻¹), A is the frequency factor (s⁻¹), E is the activation energy (J/mol), R is the ideal gas constant [8.314 J/(mol·K)], and T_a is the absolute temperature (Kelvin, K). The constants A and E are empirically derived (i.e., determined by fitting the model to data).

A modified Arrhenius model:

$$k = A T_a^b e^{-E/(RT_a)}$$

is often used with the T_a^b factor added to improve the curve fit for some classes of chemical reactions. The exponent b is a third empirical constant.

The data file `O_H2_rxn.dat` contains temperatures in the first column and reaction rates in the second column for the following reaction:

O + H₂ → OH + H

This reaction is generally included in all chemical reaction mechanisms used to model combustion of hydrocarbons.

## Tasks
For this project, you will:

1. Use the curve-fitting method of your choice to determine the values of A and E that achieve the best least-squares fit of the unmodified Arrhenius model to the data.
2. Perform a second curve-fit to determine values of A, b, and E in the modified Arrhenius model that achieve the best least-squares fit.
3. Develop figures showing both of your curve fits and report appropriate curve fit statistics to indicate the quality of each fit.
4. Compare the two models and determine which one better fits the experimental data.

## Instructions
Open the accompanying Python notebook in Google Colab to complete this project. The notebook contains starter code and guidance to help you solve the problem.

## Deliverables
Submit your completed Google Colab notebook with:
1. Working code implementing your solution
2. Results presented graphically in the notebook
3. Discussion section answering all the required questions

Be sure to review the grading rubric in Canvas to ensure you understand the project expectations.