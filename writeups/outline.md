---
title: Outline of topics to address
layout: default
permalink: /writeups/outline/
---

**Author:** Todd R. Story  
**Date Created:** 2025-08-16  
**Last Modified: 2025-08-17
**Description:**  List of topics to write up. 
**Keywords:** templates, TODO  

© 2025 Todd R. Story — All rights reserved.  
Unauthorized copying or distribution of this document, in whole or in part, is prohibited without prior written permission.

# Learning and Review Topics

## Thermodynamics and Statistical Mechanics
  - What is a partition function?
  - Where does S = k ln($\Omega$) come from?
  - Gibbs-Duhem relation
  - Ideal gas derivation from thermodynamcs perspective
    - https://chatgpt.com/c/68a1c730-f6ec-8333-852e-56841305e8f4
    - Maxwell Relations: what are they?
- Statistical Mechanics
  - $\Omega (E) = B\cdot V^{N}\cdot E^{3N/2}$ derivation
- Membrane Thermodynamics
  - 'What is really happening thermodynamically at the cell membrane.  Maybe put this discussion in the document "Discussion of Membrane Thermodynamics.
  - Donnan model study
    - Donnan Equation of State
      -As per paper "The Donnan Equilibrium: I. On teh thermodynamic foundation of the Donnan EOS," Philipse and Vrij, 2011.
      - Derivation from first (thermodynamic principles) 
- Negative Temperatures
  - Definition of Temperature
    - Spin systems 

## Mathematics
- Role of stochastic calculus in thermodynamics and statistical mechanics
  - ChatGPT list of areas in which it is used "is stochastic calculus useful for thermodynamics and/or statistical mechanics?
    - https://chatgpt.com/c/68a1c730-f6ec-8333-852e-56841305e8f4
    - Yes, stochastic calculus is very useful for thermodynamics and statistical mechanics. Key applications include:
      - Langevin SDE for Brownian motion
      - Fokker-Planck equation for probability evolution
      - stochastic thermodynamics (entropy production, fluctuation theorems)
      - Kramers' rate theory for escape rates
      - Non-equilibrium statistical mechanics (response, transport coefficients)
      - Chemical master equation for reaction networks
      - Gillespie algorithm for stochastic simulation
    - Yes, stochastic calculus is central to nonequilibrium statistical mechanics. Key points:
      - Langevin equation for particle dynamics
      - Fokker-Planck equation for probability distribution evolution
      - Jarzynski equality for free energy differences
      - Stratonovich vs Itô calculus for noise handling in modeling
      - Interpretation matters: Stratonovich preserves the chain rule, Itô adds correction.

## Questions
1. What is the relationship between thermodynamics and information theory?

---

# **Physical Chemistry – Full Multi-Level Outline with Sources**

This outline of p-chem is from ChatGPT, here is a link to the TOC of a proper textbook on the subject:

[📄 View PDF: Hammes – Physical Chemistry (TOC Only)](/writeups/sources/Hammes_Physical_Chemistry_TOC_only.pdf)

*File location:* `writeups/sources/Hammes_Physical_Chemistry_TOC_only.pdf`



## **I. Foundations**
1. **Basic Principles**
   - Units and dimensions  
       - *Physical Chemistry – Atkins & de Paula*  
       - *Physical Chemistry: A Molecular Approach – McQuarrie*  
   - Energy, work, heat  
       - *Atkins & de Paula*  
       - *McQuarrie*  
       - *An Introduction to Thermal Physics – Schroeder*  
   - State functions and path functions  
       - *Atkins*  
       - *McQuarrie*  

2. **Mathematical Tools**
   - Differential and integral calculus in thermodynamics  
       - *Mathematical Methods in the Physical Sciences – Boas*  
       - *Physical Chemistry – Atkins*  
   - Partial derivatives and Maxwell relations  
       - *Atkins*  
       - *McQuarrie*  
       - *Thermodynamics and an Introduction to Thermostatistics – Callen*  
   - Linear algebra (for quantum and spectroscopy)  
       - *Boas*  
       - *Mathematical Methods for Physicists – Arfken & Weber*  
   - Probability and statistics (for statistical mechanics)  
       - *Fundamentals of Statistical and Thermal Physics – Reif*  
       - *Statistical Mechanics – McQuarrie*  

---

## **II. Thermodynamics**
1. **Laws of Thermodynamics**
   - Zeroth law (temperature, thermal equilibrium)  
       - *Physical Chemistry – Atkins & de Paula*  
       - *An Introduction to Thermal Physics – Schroeder*  
   - First law (energy conservation)  
       - *Atkins & de Paula*  
       - *McQuarrie – Physical Chemistry: A Molecular Approach*  
       - *Callen – Thermodynamics and an Introduction to Thermostatistics*  
   - Second law (entropy, spontaneity)  
       - *Schroeder*  
       - *McQuarrie*  
       - *Callen*  
   - Third law (absolute entropy)  
       - *Atkins & de Paula*  
       - *Callen*  

2. **Pure Substances**
   - Equations of state (ideal gas, real gases)  
       - *Atkins*  
       - *McQuarrie*  
   - Phase diagrams, phase transitions  
       - *Atkins*  
       - *Smith, Van Ness & Abbott – Introduction to Chemical Engineering Thermodynamics*  
   - Clausius–Clapeyron equation  
       - *Atkins*  
       - *Callen*  

3. **Thermodynamic Potentials**
   - Internal energy \(U\), Enthalpy \(H\)  
       - *Callen*  
       - *McQuarrie*  
   - Helmholtz energy \(A\), Gibbs energy \(G\)  
       - *Callen*  
       - *McQuarrie*  
   - Natural variables, Legendre transforms  
       - *Callen*  

4. **Chemical Equilibrium**
   - Gibbs energy and equilibrium constant  
       - *Levine – Physical Chemistry*  
       - *McQuarrie*  
   - Le Châtelier’s principle  
       - *Atkins*  
   - Activity, fugacity, standard states  
       - *Levine*  
       - *Atkins*  

5. **Phase Equilibria**
   - Phase rule (Gibbs)  
       - *Atkins*  
   - Raoult’s law, Henry’s law  
       - *Atkins*  
       - *Smith, Van Ness & Abbott*  
   - Colligative properties  
       - *Atkins*  

6. **Electrochemistry**
   - Chemical potential and electrochemical potential  
       - *Hammes – Physical Chemistry for the Biological Sciences*  
       - *Alberty – Thermodynamics of Biochemical Reactions*  
   - Nernst equation  
       - *Atkins*  
       - *Hammes*  
   - Redox reactions and cell potentials  
       - *Atkins*  
       - *Bard & Faulkner – Electrochemical Methods*  
   - Membrane potentials, ionic strength corrections  
       - *Hammes*  
       - *Alberty*  
   - Proton-motive force in biological systems  
       - *Hammes*  
       - *Nicholls & Ferguson – Bioenergetics*  

---

## **III. Quantum Chemistry**
1. **Postulates of Quantum Mechanics**
   - Operators, observables, eigenvalues  
       - *McQuarrie & Simon – Physical Chemistry: A Molecular Approach*  
       - *Levine – Quantum Chemistry*  
   - Schrödinger equation  
       - *Griffiths – Introduction to Quantum Mechanics*  
       - *McQuarrie*  

2. **Simple Systems**
   - Particle in a box, harmonic oscillator, rigid rotor  
       - *McQuarrie*  
       - *Atkins*  
   - Hydrogen atom  
       - *McQuarrie*  
       - *Levine*  

3. **Approximation Methods**
   - Perturbation theory  
       - *Levine*  
       - *McQuarrie*  
   - Variational principle  
       - *McQuarrie*  
       - *Levine*  

4. **Molecular Structure**
   - Molecular orbitals, hybridization  
       - *McQuarrie*  
       - *Atkins*  
   - Spectroscopy basics (IR, UV-Vis, NMR)  
       - *Atkins*  
       - *Banwell & McCash – Fundamentals of Molecular Spectroscopy*  

---

## **IV. Statistical Mechanics**
1. **Connection to Thermodynamics**
   - Microstates, macrostates  
       - *Reif – Fundamentals of Statistical and Thermal Physics*  
       - *Huang – Statistical Mechanics*  
   - Ensembles (microcanonical, canonical, grand canonical)  
       - *Reif*  
       - *Huang*  
       - *McQuarrie – Statistical Mechanics*  
   - Partition functions  
       - *McQuarrie*  
       - *Reif*  

2. **Properties from Partition Function**
   - Internal energy, entropy, free energy  
       - *McQuarrie*  
       - *Reif*  
   - Heat capacities  
       - *McQuarrie*  
       - *Schroeder*  

3. **Applications**
   - Ideal gas from statistical mechanics  
       - *McQuarrie*  
       - *Reif*  
   - Quantum gases (Bose–Einstein, Fermi–Dirac)  
       - *Huang*  
       - *Reif*  
   - Chemical equilibrium from molecular partition functions  
       - *McQuarrie*  
       - *Reif*  

---

## **V. Chemical Kinetics & Dynamics**
1. **Rate Laws and Mechanisms**
   - Order of reaction  
       - *Atkins*  
       - *Espenson – Chemical Kinetics and Reaction Mechanisms*  
   - Complex mechanisms and steady-state approximation  
       - *Laidler – Chemical Kinetics*  
       - *Atkins*  

2. **Theories of Reaction Rates**
   - Collision theory  
       - *Atkins*  
       - *McQuarrie*  
   - Transition state theory  
       - *Laidler*  
       - *McQuarrie*  
   - RRKM theory  
       - *Laidler*  

3. **Catalysis**
   - Enzyme kinetics (Michaelis–Menten)  
       - *Hammes*  
       - *Atkins*  
   - Heterogeneous catalysis  
       - *Atkins*  

---

## **VI. Molecular Spectroscopy and Structure**
1. **Rotational, Vibrational, Electronic Spectra**
   - *Banwell & McCash – Fundamentals of Molecular Spectroscopy*  
   - *Atkins*  
   - *Herzberg – Molecular Spectra and Molecular Structure*  

2. **NMR, ESR, Mass Spectrometry**
   - *Pavia – Introduction to Spectroscopy*  
   - *Silverstein – Spectrometric Identification of Organic Compounds*  

3. **Laser spectroscopy, photochemistry**
   - *Atkins*  
   - *Banwell & McCash*  

---

## **VII. Special Topics for Life Sciences**
1. **Biochemical Thermodynamics**
   - ATP hydrolysis, coupled reactions  
       - *Hammes – Physical Chemistry for the Biological Sciences*  
       - *Alberty – Thermodynamics of Biochemical Reactions*  
   - Free energy transduction  
       - *Nicholls & Ferguson – Bioenergetics*  

2. **Electrochemical Gradients in Cells**
   - Nernst and Goldman equations  
       - *Hammes*  
       - *Alberty*  
   - Membrane potentials, ion transport  
       - *Voet & Voet – Biochemistry*  
       - *Hammes*  

3. **Macromolecular Stability**
   - Protein folding thermodynamics  
       - *Cantor & Schimmel – Biophysical Chemistry*  
       - *Hammes*  
   - Ligand binding  
       - *Hammes*  

4. **Photosynthesis and Oxidative Phosphorylation**
   - Energy coupling and efficiency  
       - *Nelson & Cox – Lehninger Principles of Biochemistry*  
       - *Nicholls & Ferguson*  

5. **Non-equilibrium Thermodynamics**
   - Steady-state fluxes in metabolism  
       - *de Groot & Mazur – Non-Equilibrium Thermodynamics*  
   - Entropy production in living systems  
       - *Hill – Free Energy Transduction and Biochemical Cycle Kinetics*  
---

# **Cell Biology – Full Multi-Level Outline with Sources**

This outline of cell biology is from ChatGPT, here is a link to the TOC of a proper textbook (Alberts et al, 5th Edition) on the subject:

[📄 View PDF: Alberts et al – Molecular Biology of the Cell (TOC/Front Matter Only)](/writeups/sources/MBoC_5Ed_FrontMatter.pdf)

*File location:* `writeups/sources/MBoC_5Ed_FrontMatter.pdf`

---

# **Biochemistry – Full Multi-Level Outline with Sources**

This outline of biochemistry is from ChatGPT, here is a link to the TOC of a proper textbook (Lehninger, 6th Edition) on the subject:

[📄 View PDF: Nelson and Cox – Principles of Biochemistry, 6th Edition (TOC/Front Matter Only)](/writeups/sources/Lehninger6thEd_FrontMatter.pdf)

*File location:* `writeups/sources/Lehninger6thEd_FrontMatter.pdf`

