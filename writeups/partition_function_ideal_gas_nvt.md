---
title: Ideal Gas Partition Function (NVT)
layout: default
permalink: /writeups/ideal_gas_partition_function_nvt/
---

**Author:** Todd R. Story  
**Date Created:** 2025-08-12  
**Last Modified:** 2025-08-12  
**Description:** Derivation of the canonical (N,V,T) partition function for a classical monatomic ideal gas.  
**Keywords:** statistical mechanics, partition function, ideal gas, canonical ensemble, thermal wavelength

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

# Partition Function of a Classical Ideal Gas (N,V,T)

We derive the canonical partition function $Z(N,V,T)$ for a monatomic classical ideal gas.

## Setup (Canonical Ensemble)

- Fixed: particle number $N$, volume $V$, temperature $T$.  
- Classical canonical partition function:

$$
Z(N,V,T) = \frac{1}{h^{3N}N!} \int d^{3N}q\, d^{3N}p\; \exp\!\big[-\beta H(p,q)\big],
\qquad \beta \equiv \frac{1}{k_B T}
\label{eq:canonical_partition_function}
$$

Here $h$ makes the phase–space integral dimensionless, and $1/N!$ enforces indistinguishability.

For an **ideal gas**, the Hamiltonian has no potential term:

$$
H(p,q) = \sum_{i=1}^{N} \frac{\mathbf p_i^2}{2m}
\label{eq:ideal_gas_hamiltonian}
$$

so the integrand in \eqref{eq:canonical_partition_function} is independent of the positions $q$.

## Position Integral

The configuration integral factorizes:

$$
\int d^{3N}q = \left(\int_V d^3q\right)^{\!N} = V^{N}
\label{eq:position_integral}
$$

## Momentum Integral

The momentum integral also factorizes:

$$
\int d^{3N}p\, e^{-\beta \sum_i \mathbf p_i^2/2m}
= \prod_{i=1}^{N}\left(\int d^{3}p_i\, e^{-\beta \mathbf p_i^2/2m}\right)
= \left[\int d^{3}p\, e^{-\beta p^2/2m}\right]^{\!N}
\label{eq:momentum_integral_factorization}
$$

In spherical momentum coordinates:

$$
d^3p = p^2 \sin\theta \; dp \; d\theta \; d\phi
\label{eq:momentum_volume_element}
$$

so:

$$
\int d^{3}p\, e^{-\beta p^2/2m}
= 4\pi \int_{0}^{\infty} p^{2} e^{-\beta p^{2}/2m}\, dp
= (2\pi m k_B T)^{3/2}
\label{eq:momentum_integral_result}
$$

## Assemble $Z$ and Define the Thermal Wavelength

Combining \eqref{eq:position_integral} and \eqref{eq:momentum_integral_result} into \eqref{eq:canonical_partition_function}:

$$
Z(N,V,T) = \frac{1}{h^{3N}N!}\, V^{N}\, \big(2\pi m k_B T\big)^{3N/2}
\label{eq:ideal_gas_partition_pre_lambda}
$$

Introduce the (de Broglie) **thermal wavelength**:

$$
\Lambda \;\equiv\; \frac{h}{\sqrt{2\pi m k_B T}}
\label{eq:thermal_wavelength}
$$

to obtain the standard compact form:

$$
\boxed{
Z(N,V,T) = \frac{1}{N!}\left(\frac{V}{\Lambda^{3}}\right)^{N}
}
\label{eq:ideal_gas_partition_final}
$$

## Consistency Checks

- **Dimensionless:** $Z$ is unitless because the phase–space measure $d^{3N}q\,d^{3N}p$ is scaled by $h^{3N}$.  
- **Extensivity:** $\ln Z \sim N$, giving $F=-k_BT\ln Z$ extensive.  
- **Ideal-gas law:** $P = -\left(\partial F/\partial V\right)_{T,N} = N k_BT / V$.  
- **Internal energy:** $U = -\partial \ln Z/\partial \beta = \tfrac{3}{2}N k_B T$ (monatomic).  

*Notes:*  
1) The classical expression assumes $n\Lambda^{3} \ll 1$ (non-degenerate gas).  
2) Quantum statistics (Bose/Fermi) replace the $1/N!$ Gibbs factor with (anti)symmetrization when degeneracy matters.
---
title: Ideal Gas Partition Function (NVT)
layout: default
permalink: /writeups/partition_function_ideal_gas_nvt/
---

**Author:** Todd R. Story  
**Date Created:** 2025-08-12  
**Last Modified:** 2025-08-12  
**Description:** Derivation of the canonical (N,V,T) partition function for a classical monatomic ideal gas.  
**Keywords:** statistical mechanics, partition function, ideal gas, canonical ensemble, thermal wavelength

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

# Partition Function of a Classical Ideal Gas (N,V,T)

We derive the canonical partition function \( Z(N,V,T) \) for a monatomic classical ideal gas.

## Setup (Canonical Ensemble)

- Fixed: particle number \( N \), volume \( V \), temperature \( T \).  
- Classical canonical partition function:
\[
Z(N,V,T)
= \frac{1}{h^{3N}N!}
\int d^{3N}q\, d^{3N}p\;
\exp\!\big[-\beta H(p,q)\big],
\qquad \beta \equiv \frac{1}{k_B T}.
\]
Here \( h \) makes the phase–space integral dimensionless, and \( 1/N! \) enforces indistinguishability.

For an **ideal gas**, the Hamiltonian has no potential term:
\[
H(p,q) = \sum_{i=1}^{N} \frac{\mathbf p_i^2}{2m},
\]
so the integrand is independent of the positions \( q \).

## Position Integral

The configuration integral factorizes:
\[
\int d^{3N}q = \left(\int_V d^3q\right)^{\!N} = V^{N}.
\]

## Momentum Integral

The momentum integral also factorizes:
\[
\int d^{3N}p\, e^{-\beta \sum_i \mathbf p_i^2/2m}
= \prod_{i=1}^{N}\left(\int d^{3}p_i\, e^{-\beta \mathbf p_i^2/2m}\right)
= \left[\int d^{3}p\, e^{-\beta p^2/2m}\right]^{\!N}.
\]
In spherical momentum coordinates,
\[
d^3p = p^2 \sin\theta \; dp \; d\theta \; d\phi,
\]
so
\[
\int d^{3}p\, e^{-\beta p^2/2m}
= 4\pi \int_{0}^{\infty} p^{2} e^{-\beta p^{2}/2m}\, dp
= (2\pi m k_B T)^{3/2}.
\]

## Assemble \( Z \) and Define the Thermal Wavelength

Putting pieces together:
\[
Z(N,V,T)
= \frac{1}{h^{3N}N!}\, V^{N}\, \big(2\pi m k_B T\big)^{3N/2}.
\]
Introduce the (de Broglie) **thermal wavelength**
\[
\Lambda \;\equiv\; \frac{h}{\sqrt{2\pi m k_B T}},
\]
to obtain the standard compact form
\[
\boxed{ \;
Z(N,V,T) \;=\; \frac{1}{N!}\left(\frac{V}{\Lambda^{3}}\right)^{\!N}
\; }.
\]

## Consistency Checks

- **Dimensionless:** \( Z \) is unitless because the phase–space measure \( d^{3N}q\,d^{3N}p \) is scaled by \( h^{3N} \).  
- **Extensivity:** \( \ln Z \sim N \), giving \( F=-k_BT\ln Z \) extensive.  
- **Ideal-gas law:** \( P = -\left(\partial F/\partial V\right)_{T,N} = N k_BT / V \).  
- **Internal energy:** \( U = -\partial \ln Z/\partial \beta = \tfrac{3}{2}N k_B T \) (monatomic).  

*Notes:*  
1) The classical expression assumes \( n\Lambda^{3} \ll 1 \) (non-degenerate gas).  
2) Quantum statistics (Bose/Fermi) replace the \( 1/N! \) Gibbs factor with (anti)symmetrization when degeneracy matters.
