---
title: S_equals_K_ln_Omega
layout: default
permalink: /writeups/S_equals_K_ln_Omega/
---

**Author:** Todd R. Story  
**Date Created:** 2025-08-19  
**Last Modified:**   
**Description:** Why does S = k x ln(Omega)?    
**Keywords:** entropy, Boltzmann, thermodynamics

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

# $S=k_{B}\cdot \ln(\Omega)$

This discussion follows Reif's book, Chapter 3, leading up to Equation 3.3.12 on Page 99.  

Consider a closed system $A^{(0)}$ consisting of two subsystems such that $A^{(0)} \equiv A+A'$ and which are in thermal contact.  The energy of the total system is such that:

$$
E^{(0)} = E+E'
$$

At this point, we have made no assumption regarding the relative sizes of the subsystems.  Let us focus on the unprimed system $A$ with energy $E$.  Since the system is closed, the total energy is $E^{0}$ and this is constant since energy must be conserved.  Subsystem A on the other hand, does not have a constant energy, since it may exchange energy with its companion system $E'$, so that:

$$
0 \leq E \leq E^{0}
\label{eq:sklogomega:possible_E_values}
$$

The question is, what is the macroscopic value of $E$, asked in the thermodynamic sense?  I.e., since strictly this value is variable we might instead inquire as to its average and deviations from its average, given that random exchanges between the two subsystems will result in fluctuations.  Two points to remember regarding what is and what is not constant:

* **NOT CONSTANT: The probability of subsystem having energy $E$**
  - Based on \eqref{eq:sklogomega:possible_E_values} the system could have an energy equal or close to zero or, on the other extreme, equal or close to the total energy $E^{0}$.  But these cases are unlikely, astronomically so in the case of the macroscopic physical world that we are ultimately talking about.  

* **CONSTANT: The probability of each system microstate**
  - This is a fundamental assumption in statistical mechanics. Thus, plot spoiler, such extreme energy states as mentioned in the previous bullet point are in theory possible but unlikely.  

The probability $P(E)$ of finding $A$ subsystem in state with energy $E=E^{(0)}-E'$ is assumed proportional to the total number of microstates available to the *total system* $A^{0}$ which in turn is proportional to the product of the respective number of microstates available to each subsystem under these conditions:

$$
P(E) = C\cdot \Omega(E^{0}) = C\cdot \Omega(E) \cdot \Omega(E^{0}-E)
$$  

$\Omega(E)$ and $\Omega(E^{0}-E)$ are extremely high increasing and decreasing functions of subsystem $A$'s energy $E$, so that the above probability exhibits a sharply peaked maximum.  Taking the natural log (WHY DO WE DO THIS?):

$$
\ln(P(E)) = \ln(C) + \ln(\Omega(E)) + \ln(\Omega(E^{0}-E))
$$  

To find the maximum, differentitate and set to zero:

$$
\begin{align}
0 &= \frac{\partial \ln(\Omega(E))}{\partial E} + \frac{\partial \ln(\Omega(E')}{\partial E} &=  \frac{\partial \ln(\Omega(E))}{\partial E} - \frac{\partial \ln(\Omega(E')}{\partial E'}
\end{align}
$$

Notice in the second term we switched from the partial with respect to $E$ to $E'$, thus since $E'=E^{0}-E$ we obtain the minus sign, thus:

$$
\frac{\partial \ln(\Omega(E))}{\partial E} = \frac{\partial \ln(\Omega(E')}{\partial E'}
$$

Defining $\beta(E) \equiv \nicefrac{\partial \ln(\Omega(E)) }{\partial E}$ the above becomes:

$$
\beta(\tilde{E})=\beta'(\tilde{E}')
$$