# Simulation Setup

# 1. Introduction

The accuracy and reliability of any Computational Fluid Dynamics (CFD) investigation depend significantly on the numerical setup adopted during the simulation. Even with an accurate physical model, inappropriate solver settings, poor mesh quality, or incorrect boundary conditions can lead to inaccurate predictions of pressure distribution, shock-wave structure, turbulence generation, and combustion characteristics.

The purpose of this document is to provide a comprehensive description of the numerical setup employed during the CFD analysis of hydrogen-fueled scramjet injector geometries. Every effort was made to maintain identical computational conditions for all injector configurations so that any observed differences in performance could be attributed solely to the injector geometry rather than numerical inconsistencies.

The three injector configurations investigated in this study were:

- Wedge Strut Injector
- Lobed Strut Injector
- Diamond Strut Injector

All simulations were carried out under identical operating conditions.

---

# 2. Computational Geometry

The computational model represents the internal flow passage of a hydrogen-fueled scramjet combustor.

The geometry consists of four major regions:

- Air inlet section
- Fuel injector (strut)
- Combustion chamber
- Outlet section

The injector is positioned inside the combustor such that hydrogen is introduced directly into the incoming supersonic airflow.

To ensure a fair comparison, the combustor dimensions remained unchanged throughout the investigation. Only the injector geometry was modified between simulations.

This approach eliminates unnecessary variables and allows the influence of injector shape to be isolated.

---

# 3. Injector Configurations

Three injector geometries were analysed.

## Wedge Strut

The wedge injector possesses a sharp leading edge that produces relatively stable oblique shock waves while generating moderate streamwise vortices. This configuration is generally known for providing a balanced compromise between pressure recovery and fuel-air mixing.

---

## Lobed Strut

The lobed injector incorporates multiple lobes designed to enhance vortex generation. The increased turbulence improves hydrogen-air mixing and combustion efficiency, although it also increases aerodynamic losses.

---

## Diamond Strut

The diamond injector produces weaker disturbances in the incoming airflow. Consequently, pressure losses are reduced, but vortex generation and turbulent mixing are comparatively weaker.

---

# 4. Working Fluid

The simulations consider two primary fluids:

## Air

Air enters the combustor at supersonic velocity and acts as the oxidizer required for hydrogen combustion.

The airflow remains compressible throughout the combustor, making density variations an important part of the numerical solution.

---

## Hydrogen

Hydrogen is selected as the fuel because it possesses several characteristics that make it suitable for scramjet propulsion.

These include:

- High specific energy
- Rapid ignition characteristics
- Fast flame speed
- Clean combustion products
- Suitability for hypersonic propulsion

The hydrogen is injected through the strut injector into the incoming supersonic airflow where mixing and combustion occur.

---

# 5. Flow Assumptions

The CFD simulations were performed under the assumptions appropriate for compressible supersonic reacting flows.

Important assumptions include:

- Compressible flow
- Continuum flow assumption
- Newtonian fluid behaviour
- Ideal gas behaviour (where applicable)
- Turbulent flow
- Steady-state numerical solution (if applicable)
- Finite-rate combustion model or equivalent combustion formulation

These assumptions are commonly adopted in numerical investigations of scramjet combustors.

---

# 6. Mesh Generation

The computational domain was discretized using a finite-volume mesh.

The primary objective of mesh generation was to accurately resolve important flow features while maintaining reasonable computational cost.

Mesh refinement was introduced in regions where steep gradients were expected.

These regions include:

- Injector leading edge
- Hydrogen injection location
- Shock-wave interaction regions
- Combustor walls
- Mixing layer
- Downstream combustion zone

Special attention was given to minimizing numerical diffusion because excessive diffusion can weaken shock structures and reduce the accuracy of combustion predictions.

Mesh quality was evaluated using standard quality indicators such as skewness and orthogonal quality to ensure numerical stability.

---

# 7. Governing Equations

The numerical simulation solves the fundamental conservation equations governing fluid flow.

These include:

## Continuity Equation

Represents conservation of mass.

---

## Momentum Equations

Represent conservation of linear momentum in each spatial direction.

---

## Energy Equation

Accounts for temperature variation, heat transfer, and energy released during combustion.

---

## Species Transport Equation

Predicts hydrogen-air mixing and chemical species distribution inside the combustor.

Together, these equations describe the coupled behaviour of compressible reacting flow.

---

# 8. Numerical Method

ANSYS Fluent employs the Finite Volume Method (FVM) for discretization.

The computational domain is divided into numerous control volumes.

For every control volume:

- Mass conservation is satisfied.
- Momentum conservation is satisfied.
- Energy conservation is satisfied.
- Species conservation is satisfied.

The algebraic equations resulting from discretization are solved iteratively until convergence.

The Finite Volume Method is widely adopted in aerospace CFD because it preserves conservation properties even for highly compressible flows involving strong shock waves.

---

# 9. Solver Selection

The density-based solver was selected because the present investigation involves compressible supersonic flow.

Density-based solvers are particularly suitable for:

- High Mach number flows
- Shock-wave prediction
- Compressible reacting flows
- Scramjet simulations

Compared with pressure-based solvers, the density-based approach provides improved numerical robustness for hypersonic applications.

---

# 10. Turbulence Modelling

The airflow inside a scramjet combustor is highly turbulent due to:

- Shock-wave interactions
- Boundary-layer development
- Hydrogen injection
- Vortex formation
- Combustion

Directly resolving every turbulent eddy would require enormous computational resources.

Therefore, an engineering turbulence model is employed to approximate the effects of turbulence while maintaining practical computational cost.

The selected turbulence model predicts turbulent viscosity and mixing behaviour, both of which strongly influence combustion efficiency.

---

# 11. Boundary Conditions

Boundary conditions define the interaction between the computational domain and its surroundings.

The principal boundaries include:

### Air Inlet

Supersonic incoming airflow enters the combustor.

---

### Hydrogen Injector

Hydrogen fuel is injected through the strut geometry.

---

### Combustor Walls

No-slip wall boundary conditions are applied.

---

### Outlet

Flow exits the computational domain through a pressure outlet or equivalent downstream boundary.

Identical boundary conditions were maintained for all injector geometries to ensure a meaningful comparison.

---

# 12. Solution Convergence

Convergence was monitored throughout every simulation.

The following parameters were observed:

- Residual reduction
- Pressure stabilization
- Velocity stabilization
- Temperature stabilization
- Mass conservation
- Overall solution stability

Only after achieving stable convergence were the numerical results accepted for analysis.

---

# 13. Post-Processing

After convergence, the numerical data were analysed using ANSYS Fluent post-processing tools.

The following contours and flow variables were investigated:

- Pressure
- Velocity
- Density
- Temperature
- Mach Number
- Turbulence
- Species Distribution

Flow vectors and streamlines were also examined to identify vortex structures and mixing behaviour.

---

# 14. Numerical Limitations

Although CFD provides extensive insight into complex flow physics, several limitations should be acknowledged.

These include:

- Dependence on turbulence models
- Approximate combustion modelling
- Mesh sensitivity
- Numerical discretization error
- Boundary condition uncertainty
- Computational cost limitations

Recognizing these limitations is essential for proper interpretation of the simulation results.

---

# 15. Summary

The simulation setup adopted in this investigation follows standard aerospace CFD practices used for the numerical analysis of scramjet combustors.

By maintaining identical numerical conditions for all injector geometries, the study provides a fair comparison of the aerodynamic and combustion performance of wedge, lobed, and diamond strut injectors.

The selected computational methodology enables accurate investigation of shock-wave formation, turbulent mixing, combustion efficiency, and pressure recovery while maintaining practical computational cost.
