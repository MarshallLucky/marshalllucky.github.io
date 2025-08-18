---
title: Microstates Function for a Monatomic Ideal Gas
layout: default
permalink: /writeups/omega_E_monatomic_ideal_gas/
---

**Author:** Todd R. Story  
**Date Created:** 2025-08-17  
**Last Modified:** 2025-08-17  
**Description:** Derivation of $\Omega_{E}$ for a monotomic ideal gas.
**Keywords:** microstate density, statistical mechanics, ideal gas, monatomic, microcanonical ensemble

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.


## Microcanonical $\Omega(E)$ for a Monatomic Ideal Gas

**Hamiltonian**

$$
H(\mathbf q,\mathbf p)=\sum_{i=1}^{N}\frac{\mathbf p_i^2}{2m}
$$

**Cumulative phase volume**

$$
\Phi(E)=\frac{1}{h^{3N}N!}\int d^{3N}q\,d^{3N}p\;\Theta\!\big(E-H(\mathbf q,\mathbf p)\big)
$$

**Position integral**

$$
\int d^{3N}q = V^{N}
$$

**Momentum-space volume (ball in $3N$ dimensions, radius $R=\sqrt{2mE}$)**

$$
\int d^{3N}p\;\Theta\!\left(E-\sum_{i=1}^{N}\frac{\mathbf p_i^2}{2m}\right)
=\frac{\pi^{\frac{3N}{2}}}{\Gamma\!\left(\frac{3N}{2}+1\right)}(2mE)^{\frac{3N}{2}}
$$

**$\Phi(E)$**

$$
\Phi(E)=\frac{V^{N}}{h^{3N}N!}\;
\frac{\pi^{\frac{3N}{2}}}{\Gamma\!\left(\frac{3N}{2}+1\right)}\,(2mE)^{\frac{3N}{2}}
$$

**Density of states $\Omega(E)=\partial_E\Phi(E)$**

$$
\Omega(E)=\frac{\partial \Phi}{\partial E}
=\frac{V^{N}}{h^{3N}N!}\;
\frac{\pi^{\frac{3N}{2}}(2m)^{\frac{3N}{2}}}{\Gamma\!\left(\frac{3N}{2}+1\right)}
\left(\frac{3N}{2}\right) E^{\frac{3N}{2}-1}
$$

**Use $\Gamma(z+1)=z\,\Gamma(z)$ and $\pi^{3N/2}(2m)^{3N/2}=(2\pi m)^{3N/2}$ to simplify**

$$
\boxed{\;
\Omega(E)=\frac{V^{N}}{h^{3N}N!}\,
\frac{(2\pi m)^{\frac{3N}{2}}}{\Gamma\!\left(\frac{3N}{2}\right)}\,
E^{\frac{3N}{2}-1}\;}
$$

**Alternative delta-shell form**

$$
\Omega(E)=\frac{1}{h^{3N}N!}\int d^{3N}q\,d^{3N}p\;\delta\!\big(E-H(\mathbf q,\mathbf p)\big)
$$

## The Role of $h^{3N}$ in Phase Space Counting

When constructing the microcanonical ensemble, the number of microstates is obtained by integrating over phase space,

$$
\int d^{3N}q \, d^{3N}p,
$$

where $d^{3N}q$ has units of length$^ {3N}$ and $d^{3N}p$ has units of momentum$^ {3N}$. The result therefore has units of

$$
\big(\text{length}^3 \cdot \text{momentum}^3\big)^N.
$$

To make the total number of states **dimensionless**, we divide by a fundamental cell size in phase space. Quantum mechanics tells us that each independent particle occupies a minimal phase space volume of $h^3$, where $h$ is **Planck’s constant**, with units of action $(\text{momentum}\times \text{length})$. For $N$ particles, this yields the factor

$$
h^{3N}.
$$

Thus the dimensionless count of microstates is obtained by

$$
\frac{1}{h^{3N}} \int d^{3N}q \, d^{3N}p.
$$

---

### Conventions
Some authors use $(2\pi\hbar)^{3N}$ instead of $h^{3N}$, since $h=2\pi\hbar$. This is simply a matter of convention and only changes the overall normalization of the state count. 

---

### Effect on Entropy
The microcanonical entropy is defined as

$$
S(E,V,N) = k_B \ln \Omega(E),
$$

with

$$
\Omega(E) \;\propto\; \frac{1}{h^{3N}}.
$$

Changing from $h^{3N}$ to $(2\pi\hbar)^{3N}$ shifts the entropy by

$$
S \;\to\; S - 3N k_B \ln(2\pi).
$$

This is an **additive constant proportional to $N$**. Crucially:

- Entropy **differences** $\Delta S$ are unaffected.  
- All thermodynamic derivatives, such as
  $$
  \frac{1}{T} = \left(\frac{\partial S}{\partial E}\right)_{V,N}, \quad
  \frac{P}{T} = \left(\frac{\partial S}{\partial V}\right)_{E,N}, \quad
  -\frac{\mu}{T} = \left(\frac{\partial S}{\partial N}\right)_{E,V},
  $$
  are unchanged.  
- Therefore, **macroscopic thermodynamics does not depend on the precise choice** of $h$ or $2\pi\hbar$.  

---

### Summary
- The factor $h^{3N}$ arises from dividing continuous phase space into quantum cells.  
- It makes the microstate count $\Omega(E)$ dimensionless.  
- It is a convention (sometimes replaced by $(2\pi\hbar)^{3N}$).  
- It affects only the absolute entropy by an additive constant.  
- **Entropy differences and all measurable thermodynamic quantities are independent of this choice.**

## Why $\Omega(E)$ Serves as the Partition Function in the Microcanonical Ensemble

In statistical mechanics, each ensemble is defined by a **partition function**, which encodes the allowed microstates and their statistical weights:

- **Canonical ensemble** (fixed $N, V, T$):
  $$
  Z(\beta, V, N) = \sum_{\text{microstates}} e^{-\beta E_i},
  $$
  where $\beta = 1/(k_B T)$.
- **Grand canonical ensemble** (fixed $\mu, V, T$):
  $$
  \mathcal{Z}(\beta, V, \mu) = \sum_{N=0}^\infty \sum_{\text{microstates}} e^{-\beta(E_i - \mu N)}.
  $$

For the **microcanonical ensemble** (fixed $E, V, N$), all microstates consistent with energy $E$ are equally probable. The corresponding "partition function" is simply the **count of allowed states**, i.e. the density of states:

$$
Z_{\text{micro}}(E, V, N) \equiv \Omega(E).
$$

---

### Normalization of Probabilities
In the microcanonical ensemble, the probability of finding the system in a particular microstate $(\mathbf{q}, \mathbf{p})$ is

$$
P(\mathbf{q}, \mathbf{p}) =
\begin{cases}
\dfrac{1}{\Omega(E)} & \text{if } H(\mathbf{q}, \mathbf{p}) = E, \\
0 & \text{otherwise}.
\end{cases}
$$

This is directly analogous to the canonical ensemble, where probabilities are normalized by the canonical partition function $Z$.

---

### Entropy from the Partition Function
Just as the canonical free energy is obtained from $Z$,

$$
F = -k_B T \ln Z,
$$

the microcanonical entropy is obtained from $\Omega(E)$,

$$
S(E,V,N) = k_B \ln \Omega(E).
$$

Thus $\Omega(E)$ plays the exact same mathematical role for the microcanonical ensemble as $Z$ does for the canonical ensemble: it is the **normalization factor of the probability distribution**, and all thermodynamic quantities follow from it.

---

### Comparison of Ensembles

| Ensemble              | Constraints               | Partition Function | Probability of Microstate | Thermodynamic Potential |
|-----------------------|---------------------------|-------------------|---------------------------|--------------------------|
| **Microcanonical**    | $N, V, E$ fixed         | $\Omega(E)$     | $1/\Omega(E)$ if $H=E$, else 0 | Entropy $S = k_B \ln \Omega$ |
| **Canonical**         | $N, V, T$ fixed         | $Z(\beta, V, N)$ | $\dfrac{e^{-\beta E_i}}{Z}$ | Free energy $F = -k_B T \ln Z$ |
| **Grand Canonical**   | $\mu, V, T$ fixed       | $\mathcal{Z}(\beta, V, \mu)$ | $\dfrac{e^{-\beta(E_i - \mu N_i)}}{\mathcal{Z}}$ | Grand potential $\Phi = -k_B T \ln \mathcal{Z}$ |
| **Isothermal–Isobaric** | $N, P, T$ fixed       | $\Delta(N,P,T)$ | $\dfrac{e^{-\beta(E_i + P V_i)}}{\Delta}$ | Gibbs free energy $G = -k_B T \ln \Delta$ |

---

### Summary
- Each ensemble has a partition function: $\Omega(E)$ for microcanonical, $Z$ for canonical, and $\mathcal{Z}$ for grand canonical.  
- These partition functions normalize the probability distribution.  
- The associated thermodynamic potential ($S, F, \Phi$) is obtained by taking the logarithm.  
- Therefore, $\Omega(E)$ **is the partition function of the microcanonical ensemble**.

## The $N,P,T$ Ensemble and the Laplace Transform

In the canonical ensemble ($N,V,T$), the partition function is

$$
Z(N,V,T) = \sum_{\text{microstates}} e^{-\beta E_i},
$$

where the volume $V$ is fixed.  

For the isothermal–isobaric ensemble ($N,P,T$), the volume is not fixed but allowed to fluctuate under an external pressure $P$. Each microstate is therefore characterized by both an energy $E_i$ and a volume $V_i$. To account for these fluctuations, the probability weight includes an extra Boltzmann factor for the $P V$ work term:

$$
\text{weight} \;\propto\; e^{-\beta(E_i + P V_i)}.
$$

Summing over microstates and volumes gives the isothermal–isobaric partition function,

$$
\Delta(N,P,T) = \sum_{i,V} e^{-\beta(E_i + P V)}.
$$

---

### Laplace Transform of the Canonical Partition Function
Notice that if we first sum over microstates at fixed volume, we obtain the canonical partition function $Z(N,V,T)$. The $N,P,T$ partition function is then

$$
\Delta(N,P,T) = \int_0^\infty dV \; e^{-\beta P V} \, Z(N,V,T).
$$

This is exactly the **Laplace transform** of the canonical partition function $Z(N,V,T)$ with respect to the volume variable $V$, with Laplace variable $\beta P$.

---

### Why a Laplace Transform?
- The canonical ensemble fixes $V$.  
- The $N,P,T$ ensemble averages over all possible $V$, weighted by the factor $e^{-\beta P V}$ that accounts for the mechanical work required to maintain constant pressure.  
- Mathematically, this averaging procedure is precisely the Laplace transform, which converts a function of $V$ into a function of its conjugate variable $\beta P$.  

---

### Gibbs Free Energy
From this partition function, the Gibbs free energy follows:

$$
G(N,P,T) = -k_B T \ln \Delta(N,P,T).
$$

Thus, just as $Z$ generates the Helmholtz free energy in the canonical ensemble, $\Delta$ generates the Gibbs free energy in the isothermal–isobaric ensemble.

---

### Sidebar: Chain of Transforms Between Ensembles
There is a unifying pattern across ensembles:

1. **Microcanonical $(N,V,E)$:** partition function is the density of states $\Omega(E)$.  

   - Probability: all states with $E$ are equally likely.  
   - Thermodynamic potential:  
     $$
     S = k_B \ln \Omega(E).
     $$

2. **Canonical $(N,V,T)$:** obtained from the microcanonical by a **Laplace transform in energy**,
   $$
   Z(N,V,T) = \int_0^\infty dE \; e^{-\beta E}\, \Omega(E).
   $$
   - Thermodynamic potential:  
     $$
     F = -k_B T \ln Z.
     $$

3. **Isothermal–Isobaric $(N,P,T)$:** obtained from the canonical by a **Laplace transform in volume**,
   $$
   \Delta(N,P,T) = \int_0^\infty dV \; e^{-\beta P V}\, Z(N,V,T).
   $$
   - Thermodynamic potential:  
     $$
     G = -k_B T \ln \Delta.
     $$

4. **Grand Canonical $(\mu,V,T)$:** obtained from the canonical by a **generating-function sum over particle number**, often described as a fugacity-weighted series:
   $$
   \mathcal{Z}(\mu,V,T) = \sum_{N=0}^\infty e^{\beta \mu N} \, Z(N,V,T).
   $$
   - This plays a role similar to a Laplace transform in $N$, with conjugate variable $\beta \mu$.  
   - Thermodynamic potential:  
     $$
     \Phi = -k_B T \ln \mathcal{Z}.
     $$

---

### Schematic Hierarchy of Ensembles

| From Ensemble            | Transform                                | To Ensemble |
|---------------------------|------------------------------------------|-------------|
| **Microcanonical** ($N,V,E$) | Laplace in $E \;\; (E \leftrightarrow \beta)$ | **Canonical** ($N,V,T$) |
| **Canonical** ($N,V,T$)      | Laplace in $V \;\; (V \leftrightarrow \beta P)$ | **Isothermal–Isobaric** ($N,P,T$) |
| **Canonical** ($N,V,T$)      | Generating function in $N \;\; (N \leftrightarrow \beta \mu)$ | **Grand Canonical** ($\mu,V,T$) |


---

### Big Picture: Connection to Legendre Transforms
This hierarchy of ensembles mirrors the structure of **Legendre transforms** in thermodynamics:

- Microcanonical ensemble ↔ internal energy $U(E,V,N)$.  
- Canonical ensemble ↔ Helmholtz free energy $F = U - TS$.  
- Isothermal–Isobaric ensemble ↔ Gibbs free energy $G = U - TS + PV$.  
- Grand canonical ensemble ↔ grand potential $\Phi = U - TS - \mu N$.  

Each new ensemble is generated by transforming in the variable that is allowed to fluctuate (energy, volume, or particle number). The partition function formalism and the Legendre-transform formalism are two sides of the same coin: one statistical, the other thermodynamic. Together, they show how **ensembles, partition functions, and thermodynamic potentials form a tightly interconnected hierarchy**.

