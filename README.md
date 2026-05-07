# Laplacian Diffusion with Local Innovation

This repository contains the code and data files for the article "Laplacian Diffusion with Local Innovation for Decentralized P--Q Voltage Control in Distribution Networks" by Diana Vieira Fernandes, Soummya Kar and Carlos Santos Silva

## Libraries

#### pandapower

```
pip install pandapower
```
L. Thurner, A. Scheidler, F. Schäfer et al, pandapower - an Open Source Python Tool for Convenient Modeling, Analysis and Optimization of Electric Power Systems, in IEEE Transactions on Power Systems, vol. 33, no. 6, pp. 6510-6521, Nov. 2018.

# Bus-Injection Representation of the Local P-Q Controller

Bus-injection equivalent of the local $P$--$Q$ voltage controller at bus $i$. Each controllable bus performs a local primal--dual update of the state variables, the raw $P$--$Q$ set-point $\mathbf w_i=(P_{\mathrm{ctrl},i},Q_{\mathrm{ctrl},i}), $ the activation variable $z_i$, and the balance multiplier $\lambda_i=(\lambda_i^P,\lambda_i^Q).$

The update uses the local objective terms from $F(x,w,z)$, the hard projected constraints on $\mathbf w_i$ and $z_i$, the state projections, and the dualized nodal-balance residual $r_i$. The D+LI state $\mathbf s_i$ provides a local estimate of the shared controllable-injection vector. The controller computes the effective set-point $\hat{\mathbf u}_i=z_i\mathbf w_i=(\hat P_i,\hat Q_i),$
and the inverter realizes it as the complex-power injection $\hat S_i^{\mathrm{ctrl}}=\hat P_i+j\hat Q_i$ at bus $i$.

  <img src="https://raw.githubusercontent.com/d-vf/D-LI/refs/heads/main/assets/pq_controller.jpg" width="50%">

 ## [Notebooks](implementation/)

A. PQ_Control_030526 [here](implementation/PQ_Control_030526)
