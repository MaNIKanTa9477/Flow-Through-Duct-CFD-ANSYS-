# Flow-Through-Duct-CFD-ANSYS-
This project simulates incompressible fluid flow through a rectangular or circular duct using ANSYS Fluent to analyze velocity profiles, pressure drops, and flow patterns. The simulation demonstrates CFD fundamentals including geometry creation, meshing, physics setup, solution initialization, and post-processing for engineering validation.​​

Objectives
Model steady-state laminar or turbulent flow in a duct with inlet velocity boundary conditions.

Evaluate key outputs: velocity contours, pressure distribution, streamlines, and energy balance checks.

Perform mesh independence study and compare results against analytical solutions like Hagen-Poiseuille for pipes.​​

Workflow Steps
Geometry: Create duct in ANSYS DesignModeler or SpaceClaim (e.g., rectangular cross-section 1m long, 0.1m x 0.05m).​​

Meshing: Generate structured/unstructured mesh in ANSYS Meshing (aim for 100k-500k elements; refine near walls for boundary layers).​

Physics Setup (Fluent):

Select pressure-based solver, steady-state, k-epsilon turbulence (or laminar).

Materials: Air/fluid from database; assign to fluid zone.

Boundaries: Velocity inlet (e.g., 5 m/s), pressure outlet, no-slip walls.​​

Solution: Initialize, run 500-1000 iterations until residuals <1e-4; monitor mass/pressure imbalances.​

Post-Processing: Contours (velocity/pressure), pathlines, reports (inlet-outlet flux), XY plots along centerline.​

Expected Results
Velocity peaks at center with parabolic profile; recirculation possible at bends/elbows. Pressure drops linearly; validate heat transfer if conjugated.
