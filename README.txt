Airfoil Performance Estimator (Thin Airfoil Theory)
Overview
This project provides a simple, interactive Python script to estimate the aerodynamic performance of airfoils based on Thin Airfoil Theory. It calculates the lift coefficient (C_L) and the moment coefficient about the quarter-chord (C_M,c/4) for various airfoil types. Designed for educational purposes and intermediate Python users, it offers a straightforward way to understand fundamental aerodynamic concepts.
Features
* Lift and Moment Estimation: Calculates C_L and C_M,c/4 based on user inputs.
* Zero-Lift Angle of Attack (alpha_L=0) Calculation: Determines the angle at which the airfoil generates no lift.
* Airfoil Type Selection:
   * Symmetric Airfoils: Idealized airfoils with no camber.
   * Generic Cambered Airfoils: Allows direct input of maximum camber fraction.
   * NACA 4-Digit Series (Approximate): Extracts maximum camber from the NACA number for simplified calculations.
* Interactive Command-Line Interface: Guides the user through airfoil selection and parameter input.
* Robust Input Handling: Includes basic error checks for user inputs to ensure data validity.
How to Run
1. Save the Code: Save the provided Python code (from airfoil_performance_estimator) as a .py file (e.g., airfoil_estimator.py).
2. Open a Terminal/Command Prompt: Navigate to the directory where you saved the file.
3. Run the Script: Execute the script using a Python interpreter:
python airfoil_estimator.py

4. Follow the Prompts: The program will guide you through selecting an airfoil type and entering the angle of attack.
Theoretical Background (Thin Airfoil Theory)
Thin Airfoil Theory is a simplified aerodynamic model that assumes:
   * The airfoil is infinitesimally thin (represented by its camber line).
   * The fluid flow is incompressible and inviscid (no friction).
   * Calculations are valid for small angles of attack.
Key Formulas:
   * Lift Coefficient (C_L): C_L=2pi(alpha−alpha_L=0)
   * Moment Coefficient about Quarter-Chord (C_M,c/4):
   * Symmetric Airfoils: C_M,c/4=0
   * Parabolic Cambered Airfoils (max camber h): alpha_L=0=−2h (radians), C_M,c/4=pih
Limitations
It's important to be aware of the limitations of this tool due to the nature of Thin Airfoil Theory and the approximations made:
   * No Drag Calculation: The theory does not account for aerodynamic drag.
   * Accuracy Range: Results are accurate only for small angles of attack (typically below 10^\\circ - 15^\\circ) and do not predict stall.
   * Idealized Flow: Does not consider real-world effects like viscosity, turbulence, or flow separation.
   * NACA 4-Digit Approximation: The NACA 4-digit implementation is a simplification, using only the maximum camber to approximate the camber line as a single parabola. Real NACA 4-digit airfoils have a more complex camber distribution.
   * Limited Airfoil Types: Only symmetric, generic parabolic cambered, and an approximated NACA 4-digit series are supported. More complex airfoil geometries (e.g., NACA 5-digit, 6-series) are not included.
This tool is best used for conceptual understanding and educational purposes rather than detailed engineering design.