# Methodology

# 1. Introduction

Computational Fluid Dynamics (CFD) has become one of the most important engineering tools for analyzing complex flow phenomena encountered in modern aerospace propulsion systems. Unlike conventional experimental techniques, CFD provides complete spatial and temporal information about flow variables such as pressure, velocity, density, temperature, turbulence intensity, and species concentration throughout the computational domain. This capability makes CFD particularly valuable for scramjet research, where direct experimental measurements inside the combustor are extremely difficult because of the high temperatures, supersonic flow velocities, and extremely short combustion residence times.

The primary objective of this research was to numerically investigate the influence of injector geometry on the aerodynamic and combustion characteristics of a hydrogen-fueled scramjet combustor. Since the injector is responsible for introducing fuel into the supersonic airstream, its geometry strongly affects shock-wave formation, vortex generation, turbulent mixing, combustion efficiency, and total pressure recovery.

Three different injector configurations—Wedge Strut, Lobed Strut, and Diamond Strut—were investigated using identical computational domains and operating conditions. Maintaining identical simulation conditions ensured that the observed differences in combustor performance resulted solely from the injector geometry rather than variations in boundary conditions or numerical settings.

The numerical methodology adopted in this study follows a systematic workflow beginning with literature review and geometry development, followed by mesh generation, selection of governing equations and physical models, numerical solution using the finite volume method, convergence assessment, and finally post-processing and comparative analysis of the simulation results.

---

# 2. Research Methodology Workflow

The complete numerical methodology adopted during this research can be summarized as follows:

1. Comprehensive literature review
2. Development of computational geometry
3. Construction of the combustor computational domain
4. Mesh generation and quality assessment
5. Selection of governing equations
6. Selection of turbulence and combustion models
7. Specification of boundary conditions
8. Configuration of numerical solver
9. Numerical simulation
10. Monitoring of convergence
11. Post-processing of CFD results
12. Comparative performance evaluation

Each stage contributes to the overall reliability and accuracy of the CFD analysis.

---

# 3. Literature Review

The investigation began with a detailed review of published literature on scramjet propulsion, hydrogen fuel injection, supersonic combustion, and computational fluid dynamics. Previous experimental and numerical studies were examined to understand the current state of research, identify commonly used injector configurations, and determine appropriate numerical methodologies.

Particular attention was given to published investigations concerning wedge, lobed, and diamond strut injectors, as these geometries have demonstrated different capabilities for generating streamwise vortices, promoting turbulent mixing, and influencing combustion efficiency.

The literature survey also provided guidance regarding:

- Computational domain construction
- Turbulence modelling approaches
- Combustion modelling strategies
- Selection of boundary conditions
- Validation techniques
- Performance parameters used for comparison

The information obtained from previous studies formed the foundation for developing the numerical model used in this investigation.

---

# 4. Geometry Development

The computational geometry was developed to represent the internal flow passage of a hydrogen-fueled scramjet combustor. The principal objective was to establish a common computational domain within which different injector geometries could be evaluated under identical operating conditions.

Three injector configurations were modelled:

## Wedge Strut

The wedge injector possesses a sharp leading edge that generates relatively stable oblique shock waves. The downstream flow experiences moderate vortex formation, promoting balanced fuel-air mixing while maintaining acceptable pressure recovery.

## Lobed Strut

The lobed injector incorporates multiple protruding lobes designed to generate strong streamwise vortices. These vortices significantly increase turbulent mixing between hydrogen and air, improving combustion efficiency but simultaneously increasing total pressure losses.

## Diamond Strut

The diamond injector features a more streamlined configuration. It produces comparatively weaker shock structures and reduced vortex strength, leading to lower aerodynamic losses but also reduced mixing effectiveness.

Using identical combustor dimensions for all three cases ensured that injector geometry remained the only independent variable in the investigation.

---

# 5. Computational Domain

The computational domain represents the internal flow region through which compressed air enters, interacts with the hydrogen injector, undergoes mixing and combustion, and finally exits the combustor.

The domain includes:

- Air inlet section
- Fuel injection region
- Supersonic combustion chamber
- Downstream outlet section

The domain dimensions were selected to ensure that shock-wave development, vortex formation, combustion processes, and downstream flow recovery could all be captured within the computational region without introducing artificial boundary effects.

A sufficiently long downstream section was maintained to allow the flow field to stabilize before reaching the outlet boundary.

---

# 6. Mesh Generation

The computational domain was discretized into a finite number of control volumes using the finite volume approach. Mesh generation represents one of the most critical stages in any CFD simulation because the governing conservation equations are solved individually within each control volume.

The mesh was generated to satisfy two primary objectives:

- Accurate resolution of steep flow gradients.
- Reasonable computational cost.

Mesh refinement was strategically introduced in regions expected to exhibit strong physical gradients, including:

- Injector leading edge
- Injector trailing wake
- Hydrogen injection region
- Combustor walls
- Shock-wave interaction regions
- High-temperature combustion zones

These regions experience rapid variations in pressure, density, velocity, and temperature. A coarse mesh in such regions can introduce excessive numerical diffusion, resulting in weakened shock structures, inaccurate vortex prediction, and reduced solution accuracy.

The final mesh represented a compromise between numerical accuracy and computational efficiency.

---

# 7. Governing Equations

The flow inside the scramjet combustor is governed by the conservation laws of fluid mechanics.

The CFD solver simultaneously solves:

- Conservation of Mass (Continuity Equation)
- Conservation of Momentum (Navier-Stokes Equations)
- Conservation of Energy
- Species Transport Equations

Because the airflow remains supersonic throughout the combustor, compressibility effects become significant. Consequently, variations in density, pressure, and temperature are fully coupled within the numerical solution.

The governing equations are discretized using the finite volume method and solved iteratively over the computational mesh until convergence is achieved.

---

# 8. Physical Modelling

The physical behaviour of the combustor was represented using numerical models capable of describing the dominant flow phenomena.

These include:

- Compressible flow modelling
- Turbulence modelling
- Hydrogen-air mixing
- Combustion modelling
- Heat release
- Species transport

The selection of appropriate physical models is essential because they directly influence prediction accuracy.

---

# 9. Numerical Solution Procedure

After defining the computational domain, mesh, material properties, and boundary conditions, the governing equations were solved using ANSYS Fluent.

The numerical procedure consisted of:

- Initialization of the solution
- Iterative solution of governing equations
- Updating flow variables
- Monitoring residual reduction
- Checking mass conservation
- Continuing iterations until convergence

The finite volume method ensures conservation of mass, momentum, and energy over every control volume in the computational domain.

---

# 10. Post-Processing

After convergence, the numerical results were analysed using the post-processing tools available in ANSYS Fluent.

Flow variables examined included:

- Static pressure
- Velocity magnitude
- Density
- Temperature
- Mach number
- Turbulence characteristics
- Species concentration
- Combustion efficiency

Contour plots and vector fields were analysed to understand the physical mechanisms responsible for differences among the three injector geometries.

Special attention was given to shock-wave structures, recirculation zones, vortex generation, and hydrogen-air mixing characteristics.

---

# 11. Comparative Performance Assessment

The final stage of the methodology involved a systematic comparison of the three injector configurations.

Performance was evaluated using several engineering criteria, including:

- Fuel-air mixing quality
- Shock-wave behaviour
- Vortex generation
- Pressure recovery
- Combustion efficiency
- Aerodynamic losses
- Overall combustor performance

Rather than focusing on a single parameter, the injectors were assessed based on their overall engineering performance. This approach recognizes that an effective scramjet injector must achieve a balance between enhanced mixing and acceptable pressure recovery.

---

# 12. Summary

The methodology adopted in this research follows internationally accepted CFD practices used in aerospace propulsion analysis. By maintaining identical computational domains, numerical settings, and operating conditions for all injector geometries, the study isolates the influence of injector shape on scramjet combustor performance.

The adopted methodology enables a detailed investigation of the complex interaction between compressible flow, shock waves, turbulence, hydrogen-air mixing, and combustion. The resulting numerical database provides valuable insight into injector design for future hypersonic propulsion systems and demonstrates the capability of CFD as an effective engineering design and research tool.
