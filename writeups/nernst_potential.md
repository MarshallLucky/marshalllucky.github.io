---
title: Nernst Potential Derivation
layout: default
permalink: /writeups/nernst_potential/
---

# Nernst Potential (NP)

**Author:** Todd R. Story  
**Date Created:** 2025-08-10  
**Last Modified:** 2025-08-10  
**Description:** Nernst Potential derivation and analysis. 
**TODO:** 
- Check sign of d_mu_electric = d_mu_chemical   
- Number equations
- Explain origin of chem potential equation
  - Origin of the natural log term
  - Relative to some standard state (but that will subtract out and or divide out (inside the ln() term))
- Ditto for electric potential
- Discussion of equilibrium nature of this relationship
**Keywords:** physics, biology, [other relevant tags]  

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

## Context
The situation is that we have a biological membrane across which:
* there is a nonzero electrical potential (voltage)
  - which is often maintained for basically independent reasons, say by the ETC within the inner chamber of mitochondria.
* there are ionic (charged) solutes on each side of the membrane:
  - some of these solutes are permeable with respect the membrane;
  - at least one solute is not permeable strictly and is also of different concentrations on each side:
    - this is what maintains the potential difference.

Without a non-permeable solute with differing concentrations, there would be no voltage. In this case, given all permeable solutes, they would just tend toward equal concentrations on each sides.  It is the imposition of an external voltage, which would be typically established via a non-permeable solute of unequal concentrations (but one might envision somehow a voltage accomplished by some other means), that makes this interesting.  

In this situation, we have two opposing tendencies:
* the tendency of unequal concentrations, in this case on the two sides of the membrane, to equalize;
* the tendency of permeable charged solutes to offset the voltage difference.

Equilibrium in this situation is defined as the concentrations at which these tendencies cancel each other out.  The equilibrium is "electrochemical" in the sense that the chemical potential, which tends to equalize concentrations of each ionic species on each side of the membrane, so that in the absence of other considerations, we would have (but we don't have this, but if we did...):

$$
[C_{i}^{\text{outside}}] = [C_{i}^{\text{inside}}]
\label{eq:trivial_equilibrium}
$$

so that the $ i^\text{th} $ concentration would be the same on both sides.  But in fact there is an imposed voltage and all permeable ionic solutes must come into equilibrium with it.

### Equilibrium

Equilibrium occurs when the chemical potential difference between the two sides is equal to the electrical potential difference between the two sides.

#### Chemical Potential

The absolute chemical potential of a solute is given by:

$$ 
\mu = \mu_{\text{0}} + R\cdot T \cdot \ln\left( [C] \right) 
\label{eq:absolute_chemical_potential}
$$

Notice this cannot be quite right because the argument of the log has units of density, see discussion in appendix below, here it does not matter because it is a question of the units of density in the log term. Since we will be taking the difference of two logs, that choice of units in effect divides out and we end up with the correct result, somewhat accidentally.

But it is the difference in this absolute potential that determines the relevant chemical potential:

$$ 
\Delta\mu = \mu_{\text{0}} + R\cdot T \cdot \ln\left( [C^{\text{outside}}] \right) - \mu_{\text{0}} - R\cdot T \cdot \ln\left( [C^{\text{inside}}] \right)
$$

so that

$$ 
\Delta\mu = R\cdot T \cdot \ln\left( \frac{[C^{\text{outside}}]}{[C^{\text{inside}}]} \right)
\label{eq:absolute_relative_potential}
$$

#### Electrical Potential
 
Similarly, the electric potential of an ionic species is:

$$
\mu_{\text{electric}} = z\cdot F\cdot \psi
\label{eq:absolute_electrical_potential}
$$

but it is the potential difference that is relevant:

$$
\begin{align*}
\Delta\mu_{\text{electric}} &= z\cdot F\cdot \psi_{\text{outside}} -  z\cdot F\cdot \psi_{\text{inside}}\\
                            &= z\cdot F\cdot \left(\psi_{\text{outside}}-\psi_{\text{inside}} \right)\\
\end{align*}
\label{eq:relative_electrical_potential}
$$ 

#### Equilibrium
Equilibrium corresponds to equal chemical and electrical potentials:

$$
\Delta\mu_{\text{electrical}} = -\Delta\mu_{\text{chemical}}
\label{eq:nernst_potential}
$$

so that

$$
z\cdot F\cdot \left(\psi_{\text{outside}}-\psi_{\text{inside}} \right) = R\cdot T \cdot \ln\left( \frac{[C^{\text{outside}}]}{[C^{\text{inside}}]} \right)
$$ 

and finally identifying the electric potential difference as the Nernst Potential:

$$
\psi_{\text{Nernst}} = \frac{R\cdot T}{z\cdot F}\cdot \ln\left( \frac{[C^{\text{outside}}]}{[C^{\text{inside}}]} \right)
$$ 

## Outstanding Questions
1. Why Gibbs free energy, i.e., why does this determine equilibrium and why does it determine whether a given reaction is spontaneous?  Is not this determined by the all-inclusive entropy change?
- [ANSWER: See section "Gibbs Free Energy"](thermodynamics.md)

2. Where does the log term come from in \eqref{eq:absolute_chemical_potential}?
- ANSWER: See appendix below.

## Appendix: Absolute Chemical Potential and the Origin of the Log Term

**Goal:** Starting from basic statistical-mechanical definitions, derive the chemical potential for the NPT ensemble, show exactly where the logarithmic term appears, and examine the dimensional consistency. We highlight that, while the final expression works in practice, there is a subtle flaw in the units analysis of the NPT partition function definition.

### Conclusions of the Following Analysis
To summarize, spoiler alert, the log term is introduced by the definition of the Gibbs free energy, which is the logarithm of the N-P-T partition function, see \eqref{nernst:eq:Gibbs_from_Delta.  The chemical potential  in turn is the derivative of the GFE with respect to N, see \eqref{nernst:eq:mu_particle}}.  In our case, we are assuming ideal conditions so that the NPT partition function is easily computed, as also shown in \eqref{nernst:eq:mu_particle}}.  Note the partial derivative is with respect to $N$ so that the natural log term, whose argument is the species concentration, is a constant inasfar as the partial is concerned.  Nevertheless, our goal was to show where the $\ln{[C]}$ came from and we have achieved this goal.

---

### 1. Basic Definitions

1. **Thermal de Broglie wavelength**  

$$
\Lambda \equiv \sqrt{\frac{h^{2}}{2\pi m k_{B}T}}, 
\quad [\Lambda] = \text{length}.
\label{nernst:eq:lambda_def}
$$

#### 1.1 Physical Meaning and Dependence

The **thermal de Broglie wavelength** $\Lambda$ represents the characteristic quantum “spread” of a particle’s position due to its thermal motion. It comes from the non-relativistic de Broglie relation $\lambda = h/p$ with the momentum scale set by the root-mean-square thermal momentum $p_{\mathrm{th}} \sim \sqrt{2\pi m k_B T}$. The result,

$$
\Lambda = \sqrt{\frac{h^{2}}{2\pi m k_B T}},
$$

shows that $\Lambda$ decreases with increasing particle mass $m$ (heavier particles have shorter thermal wavelengths) and decreases with increasing temperature $T$ (hotter particles have higher momentum and thus shorter wavelengths). For light particles at low temperatures, $\Lambda$ can become comparable to or exceed the average interparticle spacing, at which point quantum statistics (Bose–Einstein or Fermi–Dirac) become important.


2. **Canonical (NVT) partition function** for a classical ideal gas:  

$$
Z(N,V,T) = \frac{V^{N}}{N! \, \Lambda^{3N}}
\label{nernst:eq:Z_NVT}
$$

This is **dimensionless**, because $V^{N}$ (units $L^{3N}$) is canceled by $\Lambda^{3N}$ (units $L^{3N}$).

3. **NPT partition function** is defined by  

$$
\Delta(N,P,T) \equiv \int_{0}^{\infty} dV \; e^{-\beta PV} \; Z(N,V,T)
\label{nernst:eq:Delta_def}
$$

where $\beta \equiv 1/(k_B T)$ and $P$ is the external pressure.

---

### 2. Evaluating $\Delta(N,P,T)$ for an Ideal Gas

Insert Eq. $\ref{nernst:eq:lambda_def}$ and the NVT form:

$$
\Delta(N,P,T) 
= \frac{1}{N!\,\Lambda^{3N}} \int_{0}^{\infty} dV \; e^{-\beta PV} V^{N}.
\label{nernst:eq:Delta_insert}
$$

The integral is a Gamma function:

$$
\int_{0}^{\infty} e^{-\beta P V} V^{N} dV = \frac{N!}{(\beta P)^{N+1}}.
\label{nernst:eq:gamma_integral}
$$

Thus:

$$
\Delta(N,P,T) = \frac{1}{\Lambda^{3N}} \; (\beta P)^{-(N+1)}.
\label{nernst:eq:delta_final}
$$

---

### 3. Units Analysis and the Subtle Flaw

- $\Lambda$ has units $L$, so $\Lambda^{-3N}$ has units $L^{-3N}$.
- $\beta P$ has units of **number density**:

$$
\beta P = \frac{P}{k_B T} 
= \frac{nRT/V}{k_B T} 
= \frac{nR}{V k_B} 
= \frac{n N_A k_B}{V k_B} 
= \frac{N}{V},
\label{nernst:eq:betaP_to_density}
$$

where $n$ is moles, $N_A$ Avogadro's number, and $N$ particles.

Thus $\beta P$ has units $L^{-3}$.

From Eq. $\ref{nernst:eq:delta_final}$:

$$
[\Delta] = L^{-3N} \times L^{3(N+1)} = L^{3}.
\label{nernst:eq:Delta_units}
$$

So $\Delta$ has units of **volume**, not dimensionless.  
This is the flaw: the definition of $\Delta$ via the unnormalized $dV$ measure introduces an extra factor of length$^3$.

> **Comment:** To make $\Delta$ dimensionless *from the start*, the NPT definition must include a normalization factor (e.g., divide by a reference volume $V^\circ$) in the integration measure.

---

### 4. Gibbs Free Energy from $\Delta$

By definition:

$$
G(N,P,T) \equiv -k_B T \ln \Delta(N,P,T).
\label{nernst:eq:Gibbs_from_Delta}
$$

Substitute Eq. $\ref{nernst:eq:delta_final}$:

$$
G = -k_B T \left[ -3N \ln \Lambda - (N+1) \ln (\beta P) \right].
\label{nernst:eq:Gibbs_sub}
$$

This simplifies to:

$$
G = 3 N k_B T \ln \Lambda + (N+1) k_B T \ln (\beta P).
\label{nernst:eq:Gibbs_simplified}
$$

---

### 5. Chemical Potential

The **chemical potential per particle** is:

$$
\mu \equiv \left( \frac{\partial G}{\partial N} \right)_{T,P}
= 3 k_B T \ln \Lambda + k_B T \ln (\beta P).
\label{nernst:eq:mu_particle}
$$

This is **exact** for the ideal gas expression in Eq. $\ref{nernst:eq:Gibbs_simplified}$.

---

### 6. Expressing the Log Term via Concentration

From Eq. $\ref{nernst:eq:betaP_to_density}$:

$$
\beta P = \frac{N}{V} \equiv [C],
\label{nernst:eq:C_def}
$$

where $[C]$ is the **number density** (particles per volume).  

Thus:

$$
\mu = 3 k_B T \ln \Lambda + k_B T \ln [C].
\label{nernst:eq:mu_with_density}
$$

---

### 7. Molar Chemical Potential

Define the molar chemical potential $\bar{\mu} \equiv N_A \mu$. Using $R = N_A k_B$:

$$
\bar{\mu} = 3 R T \ln \Lambda + R T \ln [C].
\label{nernst:eq:mu_molar}
$$

Here, $\bar{\mu}$ is the chemical potential per mole, and $\mu$ in Eq. $\ref{nernst:eq:mu_particle}$ is per particle.

---

### 8. Dimensionality of the Log Argument

- $\Lambda$ has units of length.
- $[C]$ has units of $1/\text{length}^3$.

The combination $\Lambda^3 [C]$ is **dimensionless**:

$$
\Lambda^3 [C] \; \rightarrow \; L^{3} \times L^{-3} = 1.
\label{nernst:eq:Lambda3C_dimless}
$$

Therefore:

$$
\mu = k_B T \ln\!\big( \Lambda^3 [C] \big)
\label{nernst:eq:mu_dimless_form}
$$

is dimensionally consistent.

> **Important:** The dimensional problem is **not** with the $\mu$ expression itself — it arises earlier in $\Delta$, whose definition in NPT has leftover volume units unless normalized at the outset.

---

### 9. Summary

- The logarithmic term in $\mu$ comes from the $(\beta P)^{-(N+1)}$ factor in $\Delta$.
- Identifying $\beta P$ with number density $[C]$ makes the log term proportional to $\ln [C]$.
- For dimensional consistency, $\Lambda^3 [C]$ is the proper dimensionless log argument.
- In the NPT ensemble, $\Delta$ has volume units unless the $dV$ measure is normalized. Most derivations ignore this because additive constants in $G$ drop out of $\mu$, but rigorous analysis should ensure $\Delta$ is dimensionless from the start.

---
