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
