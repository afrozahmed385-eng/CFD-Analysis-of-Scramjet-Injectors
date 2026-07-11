# Project Summary

# CFD Analysis of Hydrogen-Fueled Scramjet Injector Geometries Using ANSYS Fluent

---

# Introduction

The development of hypersonic air-breathing propulsion systems has become one of the most active areas of aerospace research due to the growing demand for high-speed atmospheric flight, reusable launch vehicles, and next-generation defense systems. Among these propulsion technologies, the **Scramjet (Supersonic Combustion Ramjet)** has emerged as one of the most promising engines because it is capable of operating efficiently at hypersonic speeds while maintaining supersonic airflow throughout the combustion chamber.

Unlike conventional turbojet or ramjet engines, a scramjet does not slow the incoming airflow to subsonic velocities before combustion. Instead, combustion occurs while the air remains supersonic, allowing efficient operation at Mach numbers typically above Mach 5. However, this creates one of the biggest engineering challenges in propulsion engineering: achieving efficient fuel-air mixing within an extremely short residence time.

Because the airflow travels through the combustor in only a few milliseconds, the injected fuel must rapidly mix with the incoming air and burn before leaving the engine. The injector geometry therefore becomes one of the most critical design parameters in determining scramjet performance.

This research focuses on understanding how different injector geometries influence the aerodynamic and combustion characteristics inside a hydrogen-fueled scramjet combustor using Computational Fluid Dynamics (CFD).

---

# Background

Fuel injection plays a significant role in determining combustion efficiency inside a scramjet engine.

An effective injector should:

- Generate strong turbulent mixing between hydrogen and air.
- Promote rapid combustion.
- Produce stable recirculation zones.
- Minimize total pressure losses.
- Maintain efficient supersonic flow.

Different injector geometries generate different shock-wave structures, vortex systems, and turbulence levels. These flow structures directly influence combustion efficiency and pressure recovery.

To investigate these effects, three different injector geometries were selected and compared under identical operating conditions.

---

# Injector Geometries Investigated

The following injector configurations were studied:

## 1. Wedge Strut

The wedge strut generates well-defined oblique shock waves while producing stable vortices behind the injector. This configuration generally provides a good balance between fuel-air mixing and pressure recovery.

---

## 2. Lobed Strut

The lobed injector contains multiple lobes that generate stronger vortices and increased turbulent mixing. Although this improves combustion efficiency, it also increases total pressure losses because of higher turbulence intensity and shock interactions.

---

## 3. Diamond Strut

The diamond injector produces relatively weaker disturbances in the flow. Consequently, it preserves pressure better but generates weaker vortices, resulting in reduced hydrogen-air mixing and lower combustion efficiency.

---

# Objectives of the Research

The primary objectives of this project were:

- Perform Computational Fluid Dynamics (CFD) simulations of a hydrogen-fueled scramjet combustor.
- Compare the aerodynamic performance of wedge, lobed, and diamond strut injectors.
- Investigate the formation of oblique shock waves around different injector geometries.
- Study turbulent fuel-air mixing inside the combustor.
- Analyze pressure, velocity, density, temperature, and Mach number distributions.
- Evaluate combustion efficiency for each injector configuration.
- Compare pressure recovery among the three injector geometries.
- Identify the injector providing the best overall engineering performance.

---

# Software and Numerical Tools

The simulations were performed using **ANSYS Fluent**, one of the most widely used Computational Fluid Dynamics software packages in aerospace engineering.

The overall workflow consisted of:

1. Geometry creation
2. Computational domain generation
3. Mesh generation
4. Boundary condition specification
5. Selection of turbulence and combustion models
6. Numerical solution of the governing equations
7. Convergence monitoring
8. Post-processing of simulation results

---

# Engineering Concepts Involved

This project integrates concepts from multiple aerospace engineering disciplines, including:

- Computational Fluid Dynamics (CFD)
- Compressible Flow
- Gas Dynamics
- Shock Waves
- Hydrogen Combustion
- Turbulence Modeling
- Supersonic Aerodynamics
- Aerospace Propulsion
- Numerical Methods
- Thermodynamics

---

# Parameters Investigated

The performance of each injector geometry was evaluated using several important flow parameters:

- Pressure distribution
- Velocity distribution
- Density distribution
- Temperature distribution
- Mach number contours
- Shock-wave formation
- Turbulence generation
- Combustion efficiency
- Pressure recovery

These parameters provide a comprehensive understanding of the flow physics inside the scramjet combustor.

---

# Major Findings

The CFD analysis showed clear differences among the three injector geometries.

The **Wedge Strut** demonstrated the best overall performance by achieving an effective balance between fuel-air mixing and pressure recovery.

The **Lobed Strut** generated the strongest vortices, leading to excellent hydrogen-air mixing and improved combustion efficiency. However, the stronger turbulence also increased total pressure losses.

The **Diamond Strut** preserved pressure more effectively due to its streamlined geometry but generated weaker vortices, resulting in comparatively lower combustion efficiency.

These observations demonstrate that injector geometry strongly influences shock-wave formation, turbulent mixing, combustion characteristics, and overall scramjet performance.

---

# Significance of the Study

This work contributes to the understanding of injector design for hydrogen-fueled scramjet engines.

The results provide useful insights for researchers and engineers working on:

- Hypersonic propulsion
- Supersonic combustion
- CFD-based combustor design
- Hydrogen-fueled aerospace systems
- Future reusable launch vehicles
- High-speed missile propulsion

Although this study is computational in nature, it provides valuable engineering guidance before expensive experimental investigations are performed.

---

# Conclusion

This research demonstrates that injector geometry plays a fundamental role in determining the aerodynamic and combustion performance of a scramjet combustor.

Among the three configurations investigated, the wedge strut provided the best overall compromise between combustion efficiency and pressure recovery. The study highlights the importance of balancing mixing enhancement with aerodynamic losses during injector design.

The project also strengthened practical knowledge in Computational Fluid Dynamics, compressible aerodynamics, turbulence modeling, hydrogen combustion, numerical simulation, and aerospace propulsion engineering.
