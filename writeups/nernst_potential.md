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

$$ \mu = \mu_{\text{0}} + R\cdot T \cdot \ln\left( [C] \right) 
\label{eq:absolute_chemical_potential}$$

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
-[ANSWER: See section "Gibbs Free Energy"](thermodynamics.md)

2. Where does the log term come from in \eqref{eq:absolute_chemical_potential}?



### Absolute Chemical Potential Log Term