# Airfoil Performance Estimator (Thin Airfoil Theory)

## Overview
This project implements an Airfoil Performance Estimator based on Thin Airfoil Theory (TAT) to compute key aerodynamic parameters for airfoils. It allows users to estimate lift coefficient, moment coefficient, and angle of zero lift for various airfoil geometries using mathematical formulations of TAT.

## Features
- Calculates Lift Coefficient (Cl) as a function of angle of attack.
- Estimates Moment Coefficient about the quarter chord (Cm).
- Determines Angle of Zero Lift (α₀).
- Accepts camber line definition as input for customized airfoil shapes.
- Generates visual plots for performance curves.

## Requirements
- Python 3.x
- NumPy
- Matplotlib
- Jupyter Notebook (optional, for interactive use)

Install dependencies:
pip install numpy matplotlib

## Usage
1. Clone or download this repository.
2. Open `Airfoil_Performance_Estimator_(Thin_Airfoil_Theory).ipynb` in Jupyter Notebook.
3. Run the notebook cells in order.
4. Provide:
   - Airfoil camber line definition (piecewise or functional form).
   - Flow conditions (angle of attack, etc.).
5. View the computed results and plots.

## Example Output
- Cl vs. α plot.
- Cm values for different camber configurations.
- Angle of zero lift for given airfoil shape.

## Theory Background
Thin Airfoil Theory assumes:
- Small camber and thickness.
- Inviscid, incompressible, and irrotational flow.
- Linear relation between lift coefficient and angle of attack.

The lift slope for a thin airfoil is given by:
Cl = 2π (α - α₀)

## Applications
- Preliminary airfoil design.
- Academic study of aerodynamic theory.
- Performance comparison of different camber configurations.

## License
This project is open-source and available under the MIT License.
