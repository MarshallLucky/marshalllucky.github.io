---
title: Nernst Potential Derivation
layout: default
permalink: /writeups/nernst_derivation_with_gibbs_discussion/
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

2. Where does the log term come from in \eqref{eq:absolute_chemical_potential}?

### Gibbs Free Energy (GFE)
The claim is that reactions (or more generally, 'actions' period) are spontaneous *under conditions of constant temperature and constant pressure* if and only if the GFE change is negative.  Put another way, if there is positive GFE, reactions will go forward. Perhaps we can think of  GFE as a generalized fuel (that can take negative values) for a vehicle that will always 'go' if it has said fuel.

#### Proof Using Second Law
The second law states that reactions can and will occur if and only if the *total* entropy of the universe increases as a consequence of that action:

$$
\Delta S_{\text{total}} \equiv \Delta S_{\text{system}} + \Delta S_{\text{surroundings}} \geq 0
\label{eq:second_law}
$$

**Outline of Proof** Under conditions of constant temperature and pressure, we will show the Second Law \eqref{second_law} implies or is equivalent to the claim. *I.e.*, that if the total entropy change is positive then the GFE change is negative.
$$
   Delta S_{\text{total}} \geq \Leftrightarrow \delta G \leq 0
   \label{eq:equivalence_second_law_to_negative_gfe_change}
$$ 

*Proceeding...*, first recognize the heat absorbed by the surroundings \footnote{By which we mean the rest of the universe but practically speaking we can probably limit this to Earth and possibly even the lab table.} equals that produced by the system:
\footnote{This follows from other aspects of basic thermodynamics, but even right now I do not understand why the universe entropy is solely related to the heat and not to physical work.  But its freshman physics that i just need to review later.} 
\footnote{Actually some of the heat can remain in the system but nevermind all these complications.}
$$
   Delta S_{\text{surroundings}} = -\frac{\Delta Q_{system}}{T}
   \label{eq:heat_absorbed_by_surroundings}
$$
with the negative sign reflecting that heat absorbed by the surroundings is the negative of that emitted by the system (*i.e.*, the subscript "system" is not a typo). We may thus write:
$$
\Delta S_{\text{system}} + \Delta S_{\text{surroundings}} =
\Delta S_{\text{system}} - \frac{\Delta Q_{system}}{T}
\label{eq:second_law}
$$



### Absolute Chemical Potential Log Term