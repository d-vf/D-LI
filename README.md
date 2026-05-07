# Laplacian Diffusion with Local Innovation

This repository contains the code and data files for the article "Laplacian Diffusion with Local Innovation for Decentralized P--Q Voltage Control in Distribution Networks" by Diana Vieira Fernandes, Soummya Kar and Carlos Santos Silva

Pre-print: [arXiv]() 

## Libraries

#### pandapower

```
pip install pandapower
```
L. Thurner, A. Scheidler, F. Schäfer et al, pandapower - an Open Source Python Tool for Convenient Modeling, Analysis and Optimization of Electric Power Systems, in IEEE Transactions on Power Systems, vol. 33, no. 6, pp. 6510-6521, Nov. 2018.

## Simulation

### Data

#### Network

* CIGRE low voltage radial distribution network (44 bus system)
  
  <img src="https://raw.githubusercontent.com/d-vf/Var_Volt_Control//main/assets/network_44_WB_var_volt_png.png" alt="network_44" width="50%">

### Voltage drop - Baseline (Non-intervention)

  <img src="https://raw.githubusercontent.com/d-vf/Var_Volt_Control//main/assets/bus_voltage_profile_before_png.png" alt="network_44" width="50%">

### Voltage drop - Intervention
 <img src="https://raw.githubusercontent.com/d-vf/Var_Volt_Control//main/assets/bus_voltage_profile_after_png.png" alt="network_44" width="50%">

### Predicted vs. Validated Voltages

 <img src="https://raw.githubusercontent.com/d-vf/Var_Volt_Control//main/assets/plotly_voltage_comparison_png.png" alt="network_44" width="50%">

 ## [Notebooks](implementation/)

A. Var_Volt_Control_310725.ipynb [here](implementation/Var_Volt_Control_310725.ipynb)








# D-LI
