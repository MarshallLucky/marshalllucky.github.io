---
title: Enthalpy Etc
layout: default
permalink: /writeups/enthalpy_etc/
---

# Thermodynamics

## Enthalpy

**Author:** Todd R. Story  
**Date Created:** 2025-08-11  
**Last Modified:** 2025-08-12
**Last Change:** Moved Gibbs Free Energy discussion to this document.  
**Description:** Demonstration that enthalpy is heat absorbed under conditions of constant pressure.    
**Keywords:** enthalpy, thermodynamics, physics

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

## Enthalpy is Heat Absorbed under Constant Pressure
Claim: The change in enthalpy, $ \Delta H $ is the heat absorbed (or released) by a system that undergoes a state change under conditions of constant pressure.  To see this, note that enthalpy is defined as:

$$ H = E + P \cdot V $$

so that the enthalpy change due to the state change is:

$$ 
\Delta H = \Delta E + P \cdot \Delta V 
\label{eq:enthalpy_differential}
$$

but what is $ \Delta E $ ?  It is the change in the internal energy of the system which is in turn equal to the heat absorbed less the work done by the system:

$$ \Delta E = q + w = q - P \cdot \Delta V $$

where again we are assuming $ \Delta P = 0 $ since the state change is assumed to take place under conditions of constant pressure.  Let us now use this last relation to rexpress the enthalpy change as:

$ \Delta H = \Delta E + P \cdot \Delta V = q - P \cdot \Delta V + P \cdot \Delta V $

and thus we arrive at our original claim that the enthalpy is the amount of heat absorbed by the system as a consequence of a state change, i.e., the energy change of the system due to heat absorbed, only:

$ \Delta H = q $.

## Free Energy

### Gibbs Free Energy (GFE)
The claim is that reactions (or more generally, 'actions' period) are spontaneous *under conditions of constant temperature and constant pressure* if and only if the GFE change is negative.  Put another way, if there is positive GFE, reactions will go forward. Perhaps we can think of  GFE as a generalized fuel (that can take negative values) for a vehicle that will always 'go' if it has said fuel.

#### Proof Using Second Law
The second law states that reactions can and will occur if and only if the *total* entropy of the universe increases as a consequence of that action:

$$
\Delta S_{\text{total}} \equiv \Delta S_{\text{system}} + \Delta S_{\text{surroundings}} \geq 0
\label{eq:second_law}
$$

**Outline of Proof**

Under conditions of constant temperature and pressure, we will show a negative Gibbs free energy change is equivalent to and follows logically from \eqref{eq:second_law}:

$$
   \Delta S_{\text{total}} \geq 0 \; \Leftrightarrow \; \Delta G \leq 0
   \label{eq:equivalence_second_law_to_negative_gfe_change}
$$ 

**Proceeding**

First recognize the heat absorbed by the surroundings (by which we mean strictly the rest of the universe outside the system of interest) equals that produced by the system:

$$
   \Delta S_{\text{surroundings}} = -\frac{\Delta Q_{system}}{T}
   \label{eq:heat_absorbed_by_surroundings}
$$

with the negative sign reflecting that heat absorbed by the surroundings is the negative of that emitted by the system (subscript "system" is *not* a typo). We may thus write:

$$
\Delta S_{\text{system}} + \Delta S_{\text{surroundings}} =
\Delta S_{\text{system}} - \frac{\Delta Q_{system}}{T}
\label{eq:entropy_condition_in_terms_system_heat}
$$

Recognizing that system enthalpy equals the heat absorbed by it (the system), $\Delta H_{system} = \Delta Q_{system}$, and also multiplying through by negative $T$ we obtain:

$$
\Delta H_{system} - T \cdot \Delta S_{system} \leq 0
\label{eq:gibbs_change_equivalent}
$$

Note the reversal of the greater than or equal to less than or equal. Next Recall the Gibbs free energy can rbe written as (or possibly taken as *defined* as):

$$
G = H - T \cdot S
$$

Since $T$ is assumed constant, the differential form is $\Delta G=\Delta H-T\cdot \Delta S$ so that we may reexpress \eqref{eq:gibbs_change_equivalent} as 

$$
\Delta G_{system} \leq 0
$$

which proves \eqref{eq:equivalence_second_law_to_negative_gfe_change}.

### Helmholtz Free Energy
Under conditions of constant pressure and temperature, the condition for spontaneity is a negative Gibbs free energy change.  If volume is constant instead of pressure, the condition is that the *Helmholtz* free energy is negative.  The derivation is highly similar but there are some important conceptual physical differences.  

In the Gibbs case, we identified the heat absorbed by the system as the enthalpy (indeed this can be considered the definition of enthalpy). As noted in Equation \eqref{eq:enthalpy_differential} above, enthalpy just adds back the work component of the total internal energy change, leaving only the heat contribution.  This is what the surrounding environment absorbs and is what determines its entropy change, see \eqref{eq:second_law}.  In the Helmholtz case, $V$ is constant and there is no work, *i.e.*, the internal energy change $\Delta E$ is already pure heat and there is nothing to subtract.  Hence in the Helmholtz case we work directly with $E$ and $\Delta E$ instead of enthalpy.


**Outline of Helmholtz Proof** 

Under conditions of constant temperature and *volume*, we will show a negative *Helmholtz* free energy change is equivalent to and follows logically from \eqref{eq:second_law}:

$$
   \Delta S_{\text{total}} \geq 0 \; \Leftrightarrow \; \Delta F \leq 0
   \label{eq:equivalence_second_law_to_negative_hfe_change}
$$ 

**Proceeding**

Again, as in the Gibbs case, the heat absorbed by the surroundings equals that produced by the system, see \eqref{eq:heat_absorbed_by_surroundings}.  Thus we have again Equation \eqref{eq:entropy_condition_in_terms_system_heat}.  In this case, however, instead of using enthalpy, in the constant volume case we recognize the heat absorbed by the system as the internal energy change directly, $\Delta E_{system} = \Delta Q_{system}$, and thus write the next equations in such terms:

$$
\Delta E_{system} - T \cdot \Delta S_{system} \leq 0
\label{eq:helmholtz_change_equivalent}
$$

which is analogous to \eqref{eq:gibbs_change_equivalent} except we now identify the Helmholtz free energy:

$$
F = E - T \cdot S
$$

the differential form of which is now $\Delta F=\Delta E-T\cdot \Delta S$ so that we may reexpress \eqref{eq:helmholtz_change_equivalent} as 

$$
\Delta F_{system} \leq 0
$$

which proves \eqref{eq:equivalence_second_law_to_negative_hfe_change}.


