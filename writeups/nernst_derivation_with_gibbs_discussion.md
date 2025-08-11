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
**Keywords:** physics, biology, [other relevant tags]  

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

## Context
The situation is that we have a biological membrane on either side of which we have distinct ion concentrations of various species.  The concentration of each respective ion species differs from one side of the membrane to the other (and from the other species in general, but that is not what we are talking about).  Strictly, the membrane or "wall" or "barrier" does not have to be biological but it is one context in which the Nernst Potential (NP henceforth) is encountered.  

The ion species in question is by definition charged.  If it was not charged and if the membrane was permeable to that species

From a thermodynamic perspective, in the absence of opposiung forces,we would expect ions to move across the  membrane (when channels exist that facilitate this)

The **Nernst Potential** corresponds to 

there is a chemical potential inside and another outside and there is their difference.  similarly for the electrical potential, there is a difference.  these potential difference, chemical and electrical, are opposing.  when the chemical potential difference between the two sides equals the electrical potential difference between the two sides, this is the definition of equilibrium and the electrical potential in that state is the so-called Nernst potential, no?


# Gibbs Free Energy

## Entropy change 
Experienced data scientist with a passion for machine learning and mathematical derivations. Skilled in Python, R, and statistical modeling. Seeking opportunities to apply analytic abilities in innovative projects.

## Activity and Chemical Potential
The chemical potential of a given solute, say the ith, is stated in terms of its "activity," which we may think of as the amount of energy necessary to achieve the respective concentration relative to a standard concentration, all else constant (pressure, temperature, concentrations of other solutes ($ i \neq j $)

## Enthalpy
Claim: The change in enthalpy, $ \Delta H $ is the heat absorbed (or released) by a system that undergoes a state change under conditions of constant pressure.  To see this, note that enthalpy is defined as:

$ H = E + P \cdot V $

so that the enthalpy change due to the state change is:

$ \Delta H = \Delta E + P \cdot \Delta V $

but what is $ \Delta E $?  It is teh change in the internal energy of the system which is in turn equal to the heat absorbed less the work done by the system:

$ \Delta E = q + w = q - P \cdot \Delta V $ \

where again we are assuming $ \Delta P = 0 $ since the state change is assumed to take place under conditions of constant pressure.  Let us now use this last relation to rexpress the enthalpy change as:

$ \Delta H = \Delta E + P \cdot \Delta V = q - P \cdot \Delta V + P \cdot \Delta V $

and thus we arrive at our original claim that the enthalpy is the amount of heat absorbed by the system as a consequence of a state change, i.e., the energy change of the system due to heat absorbed, only:

$ \Delta H = q $.
