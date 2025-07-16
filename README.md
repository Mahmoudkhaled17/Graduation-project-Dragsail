#  CubeSat Drag Sail Simulation for Satellite Deorbiting
## Project Overview
This project presents the design and simulation of a deployable drag sail system integrated into a 3U CubeSat (4 kg) to accelerate satellite deorbiting using passive aerodynamic forces in Low Earth Orbit (LEO).

With the increasing concern over space debris, passive deorbiting techniques like drag sails provide an efficient, low-mass, fuel-free alternative to traditional propulsion systems. This simulation evaluates the performance of a drag sail across various altitudes and environmental conditions.

## Objectives
Design a 1.7 m² drag sail mechanism for a CubeSat mission.

  Simulate and analyze the satellite’s orbital decay under:

    -Earth gravity

    -Atmospheric drag

    -Solar Radiation Pressure (SRP)

    -Third-body gravity (Moon)

    -Compare orbital decay with and without drag sail across altitudes.

Use simulation data for validation and parametric study.

## Tools Used
    STK (Systems Tool Kit) – Orbit propagation, force modeling, mission simulation.

    Excel – Raw data formatting and preprocessing.



## 📊 Simulation Parameters

| Parameter           | Value                     |
|--------------------|---------------------------|
| Satellite Mass     | 4 kg                      |
| CubeSat Size       | 3U                        |
| Drag Sail Area     | 1.7 m² (also tested 3, 5 m²) |
| Drag Coefficient   | 2.0 (constant)            |
| Altitude Range Tested | 300 km – 900 km        |

## 📈 Results
Decay Time Comparison with and without drag sail:

Altitude (km)	With Drag Sail (years)	Without Drag Sail
|Altitude (km) | Value 1 | Value 2|
|300           | 0.001   | 0.21|
|500           | 0.044   | 12|
|600           | 0.34    | Not Decay|
|700           | 1.3     | Not Decay|
|800           | 9.4     | Not Decay|
|900           | 18.5    | Not Decay|

A significant reduction in orbital lifetime was observed at all altitudes.

Without a drag sail, satellites may remain in orbit indefinitely, increasing collision risk.

## 📎 Files Included
simulation_data.csv: STK exported force data (Drag, Gravity, SRP) over time and altitude.

decay_comparison_plot.png: Decay time vs altitude comparison.

drag_sail_simulation.ipynb: Python notebook for plotting & data analysis.

README.md: Project documentation.

## ✅ Outcomes
Demonstrated the efficiency of drag sails in reducing orbital lifetime.

Verified how drag area, altitude, and mass affect deorbit time.

Supported space debris mitigation efforts using low-cost, passive methods.
