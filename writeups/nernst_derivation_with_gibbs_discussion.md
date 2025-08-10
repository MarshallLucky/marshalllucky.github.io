---
title: Basic Thermodynamics
layout: default
permalink: /writeups/nernst_derivation_with_gibbs_discussion/
---

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
