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

$ H = E + P \cdot V $

so that the enthalpy change due to the state change is:

$ \Delta H = \Delta E + P \cdot \Delta V $

but what is $ \Delta E $ ?  It is the change in the internal energy of the system which is in turn equal to the heat absorbed less the work done by the system:

$ \Delta E = q + w = q - P \cdot \Delta V $

where again we are assuming $ \Delta P = 0 $ since the state change is assumed to take place under conditions of constant pressure.  Let us now use this last relation to rexpress the enthalpy change as:

$ \Delta H = \Delta E + P \cdot \Delta V = q - P \cdot \Delta V + P \cdot \Delta V $

and thus we arrive at our original claim that the enthalpy is the amount of heat absorbed by the system as a consequence of a state change, i.e., the energy change of the system due to heat absorbed, only:

$ \Delta H = q $.

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
