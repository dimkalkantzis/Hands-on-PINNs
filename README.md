# Hands-on-PINNs

## 📌 Summary
This repository explores **numerical** and **physics-informed neural approaches** to solving **partial differential equations (PDEs)**.  
We compare classical solvers with deep learning–based PINNs and their improved variants (IPINNs).  

- **1D Burgers’ equation** solved with:
  - Finite Difference Method (**FDM**)  
  - Physics-Informed Neural Networks (**PINNs**)  
  - Improved PINNs (**IPINNs**)  

- **Navier–Stokes equations** solved with:
  - Improved PINNs (**IPINNs**)  

The project provides both implementations and benchmarks to help researchers and students understand the strengths and limitations of each method.

---

## 📘 Mathematical Formulation

### 1. 1D Burgers’ Equation
The viscous Burgers’ equation:

$$
\frac{\partial u}{\partial t} 
+ u \frac{\partial u}{\partial x} 
= \nu \frac{\partial^2 u}{\partial x^2}, 
\quad x \in [0,1], \; t > 0
$$

Initial and boundary conditions:

$$
u(x,0) = -\sin(\pi x), 
\quad u(0,t) = u(1,t) = 0
$$

---

### 2. Navier–Stokes Equations
Incompressible 2D Navier–Stokes:

$$
\frac{\partial \mathbf{u}}{\partial t} 
+ (\mathbf{u} \cdot \nabla)\mathbf{u} 
= -\nabla p + \nu \nabla^2 \mathbf{u},
$$

$$
\nabla \cdot \mathbf{u} = 0
$$

where \( \mathbf{u} = (u,v) \) is velocity and \( p \) is pressure.

---

## 🧰 Methods Implemented

1. **Finite Difference Method (FDM)** – baseline discretization  
2. **Physics-Informed Neural Networks (PINNs)** – enforce PDEs in training loss  
3. **Improved PINNs (IPINNs)** – modified loss/training strategies for better stability  

---



