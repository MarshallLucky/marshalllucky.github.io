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

# **Cell Biology – Full Multi-Level Outline with Sources and Overlap Points**

---

## **I. Introduction to Cells**
1. **Fundamental Concepts**
   - The cell as the basic unit of life  
       - *Molecular Biology of the Cell – Alberts et al.*  
       - *Essential Cell Biology – Alberts et al.*  
   - History of cell theory  
       - *Alberts*  
       - *Karp – Cell and Molecular Biology*  
   - Overview of cell types (prokaryotic, eukaryotic)  
       - *Alberts*  
       - *Lodish – Molecular Cell Biology*  
   - Overlap with Physical Chemistry  
       - Thermodynamics and energy transduction in cells (*Atkins*, *Hammes*)  

2. **Chemistry of Life**
   - Water and noncovalent interactions  
       - *Alberts*  
       - *Lehninger Principles of Biochemistry – Nelson & Cox*  
   - pH, buffers, and biological relevance  
       - *Hammes – Physical Chemistry for the Biological Sciences*  
   - Macromolecules: proteins, nucleic acids, polysaccharides, lipids  
       - *Alberts*  
       - *Voet & Voet – Biochemistry*  

---

## **II. Cell Chemistry and Bioenergetics**
1. **Biological Macromolecules**
   - Structure and properties of amino acids, nucleotides, sugars, lipids  
       - *Alberts*  
       - *Lehninger*  

2. **Enzymes and Catalysis**
   - Enzyme structure, active sites, cofactors  
       - *Alberts*  
       - *Berg – Biochemistry*  
   - Kinetics: Michaelis–Menten and regulation  
       - *Hammes – Physical Chemistry for the Biological Sciences*  
       - *Laidler – Chemical Kinetics*  
   - Overlap: Chemical kinetics and transition-state theory (*Atkins*, *McQuarrie*)  

3. **Energy Conversion**
   - Laws of thermodynamics in cells  
       - *Alberts*  
       - *Hammes*  
   - Free energy, coupled reactions, and metabolic pathways  
       - *Alberts*  
       - *Lehninger*  
   - Overlap: ΔG, ΔH, ΔS relationships (*Callen*, *Atkins*)  

---

## **III. Cell Structure and Organization**
1. **Plasma Membrane**
   - Lipid bilayer, membrane proteins  
       - *Alberts*  
       - *Lodish*  
   - Membrane dynamics and transport mechanisms  
       - *Alberts*  
       - *Hammes*  
   - Overlap: Electrochemical potentials and Nernst equation (*Hammes*, *Alberty*)  

2. **Internal Membranes and Organelles**
   - ER, Golgi, vesicular trafficking  
       - *Alberts*  
       - *Karp*  
   - Lysosomes, peroxisomes  
       - *Alberts*  
   - Mitochondria and chloroplasts  
       - *Alberts*  
       - *Nicholls & Ferguson – Bioenergetics*  
   - Overlap: Proton-motive force and chemiosmosis (*Hammes*, *Alberty*)  

---

## **IV. Genetic Information**
1. **DNA Structure and Replication**
   - DNA double helix, chromatin  
       - *Alberts*  
       - *Watson – Molecular Biology of the Gene*  
   - Replication mechanisms and enzymes  
       - *Alberts*  

2. **RNA and Transcription**
   - RNA polymerases, transcription factors  
       - *Alberts*  
       - *Lodish*  

3. **Protein Synthesis**
   - Ribosomes, tRNAs, initiation/elongation/termination  
       - *Alberts*  
       - *Berg – Biochemistry*  

4. **Regulation of Gene Expression**
   - Epigenetics, chromatin remodeling  
       - *Alberts*  
       - *Kornberg – Chromatin Structure*  

---

## **V. Membrane Transport and Signal Transduction**
1. **Transport Mechanisms**
   - Passive diffusion, facilitated transport  
       - *Alberts*  
       - *Hammes*  
   - Active transport and ATP-driven pumps  
       - *Alberts*  
       - *Hille – Ion Channels of Excitable Membranes*  
   - Overlap: Gibbs energy and electrochemical gradients (*Hammes*, *Alberty*)  

2. **Cell Signaling**
   - Receptor types: GPCR, RTK  
       - *Alberts*  
       - *Lodish*  
   - Second messenger systems  
       - *Alberts*  
   - Overlap: Thermodynamic limits of signaling and binding kinetics (*Hammes*)  

---

## **VI. Cytoskeleton and Intracellular Transport**
1. **Actin Filaments**
   - Structure, treadmilling, regulation  
       - *Alberts*  

2. **Microtubules and Motors**
   - Kinesin, dynein, intracellular trafficking  
       - *Alberts*  
       - *Howard – Mechanics of Motor Proteins and the Cytoskeleton*  
   - Overlap: Free energy from ATP hydrolysis powering mechanical work (*Hammes*)  

3. **Intermediate Filaments**
   - Structural support  
       - *Alberts*  

---

## **VII. Cell Cycle, Division, and Death**
1. **Cell Cycle Regulation**
   - Cyclins, CDKs, checkpoints  
       - *Alberts*  

2. **Mitosis and Meiosis**
   - Chromosome segregation  
       - *Alberts*  

3. **Apoptosis and Autophagy**
   - Pathways and significance  
       - *Alberts*  

---

## **VIII. Intercellular Communication and Development**
1. **Extracellular Matrix and Cell Adhesion**
   - Integrins, ECM components  
       - *Alberts*  

2. **Cell–Cell Junctions**
   - Tight junctions, desmosomes, gap junctions  
       - *Alberts*  

3. **Developmental Programs**
   - Differentiation and morphogenesis  
       - *Gilbert – Developmental Biology*  
       - *Alberts*  

---

## **IX. Specialized Cells and Systems**
1. **Neurons**
   - Membrane excitability and synaptic transmission  
       - *Kandel – Principles of Neural Science*  
       - *Hille*  
   - Overlap: Action potentials and Nernst/Goldman equations (*Hammes*)  

2. **Immune System Cells**
   - Innate and adaptive immunity basics  
       - *Janeway’s Immunobiology – Murphy*  
       - *Alberts*  

---

## **X. Experimental Methods in Cell Biology**
1. **Microscopy Techniques**
   - Light, fluorescence, and electron microscopy  
       - *Alberts*  

2. **Molecular Techniques**
   - CRISPR, RNAi, recombinant DNA  
       - *Alberts*  
       - *Lodish*  

3. **Systems Approaches**
   - Genomics, proteomics, single-cell analysis  
       - *Alberts*  

---

### **Key Overlap Points with Physical Chemistry**
- **Bioenergetics:** Gibbs free energy, chemical potentials (ATP hydrolysis, redox)  
- **Electrochemistry:** Nernst equation, membrane potentials, proton-motive force  
- **Kinetics:** Enzyme mechanisms, Michaelis–Menten vs transition-state theory  
- **Thermodynamics:** Entropy in folding, stability of macromolecules, osmotic pressure  
- **Spectroscopy:** NMR and fluorescence for structural biology  


---

# **Biochemistry – Full Multi-Level Outline with Sources**

This outline of biochemistry is from ChatGPT, here is a link to the TOC of a proper textbook (Lehninger, 6th Edition) on the subject:

[📄 View PDF: Nelson and Cox – Principles of Biochemistry, 6th Edition (TOC/Front Matter Only)](/writeups/sources/Lehninger6thEd_FrontMatter.pdf)

*File location:* `writeups/sources/Lehninger6thEd_FrontMatter.pdf`
---

## **I. Foundations of Biochemistry**
1. **Cellular Foundations**
   - Cell structure and compartments  
       - *Lehninger Principles of Biochemistry – Nelson & Cox*  
       - *Voet & Voet – Biochemistry*  
   - Domains of life and evolutionary foundations  
       - *Lehninger*  
       - *Berg, Tymoczko & Gatto – Biochemistry*  
   - Overlap: Physical chemistry of membranes and diffusion (*Atkins*)  

2. **Chemical and Physical Principles**
   - Biomolecules: structure and functional groups  
       - *Lehninger*  
       - *Hammes – Physical Chemistry for the Biological Sciences*  
   - Dynamic steady state vs equilibrium  
       - *Lehninger*  
       - *Callen – Thermodynamics*  
   - Overlap: Thermodynamics and free energy in metabolism (*Atkins*)  

3. **Water and Aqueous Chemistry**
   - Hydrogen bonding, solvation, and weak interactions  
       - *Lehninger*  
       - *Hammes*  
   - Ionization, pH, and buffers (Henderson–Hasselbalch)  
       - *Lehninger*  
       - *Hammes*  
   - Overlap: pKa and buffer theory (*Atkins*)  

---

## **II. Structure and Catalysis**
1. **Amino Acids, Peptides, and Proteins**
   - Structure, properties, and classification of amino acids  
       - *Lehninger*  
       - *Berg*  
   - Peptides and covalent modifications  
       - *Lehninger*  

2. **Protein Structure**
   - Primary, secondary, tertiary, quaternary structures  
       - *Lehninger*  
       - *Cantor & Schimmel – Biophysical Chemistry*  
   - Protein folding and misfolding (prions)  
       - *Lehninger*  

3. **Protein Function**
   - Ligand binding and cooperativity (e.g., hemoglobin)  
       - *Lehninger*  
       - *Hammes*  
   - Immunoglobulins and immune system basics  
       - *Lehninger*  

4. **Enzymes**
   - Catalytic principles and mechanisms  
       - *Lehninger*  
       - *Hammes*  
   - Michaelis–Menten kinetics and inhibition  
       - *Lehninger*  
       - *Hammes*  
   - Transition-state theory  
       - *Hammes*  
       - *Atkins – Physical Chemistry*  
   - Overlap: Reaction rate theory and thermodynamics of activation (*Hammes*, *Atkins*)  

5. **Carbohydrates and Glycobiology**
   - Monosaccharides, polysaccharides, glycoconjugates  
       - *Lehninger*  
       - *Voet & Voet*  

6. **Nucleotides and Nucleic Acids**
   - Nucleotide structure, nucleic acids, DNA/RNA properties  
       - *Lehninger*  

7. **Lipids**
   - Fatty acids, triacylglycerols, phospholipids, steroids  
       - *Lehninger*  

8. **Biological Membranes and Transport**
   - Membrane architecture and transport mechanisms  
       - *Lehninger*  
       - *Hille – Ion Channels of Excitable Membranes*  
   - Overlap: Nernst equation, ΔG of ion transport (*Hammes*)  

9. **Biosignaling**
   - Receptor types, second messengers, signaling cascades  
       - *Lehninger*  

---

## **III. Bioenergetics and Metabolism**
1. **Principles of Bioenergetics**
   - Free energy changes in biological reactions  
       - *Lehninger*  
       - *Hammes*  
   - Phosphoryl group transfers and ATP hydrolysis  
       - *Lehninger*  
   - Overlap: Gibbs energy, coupling, and redox potentials (*Atkins*, *Hammes*)  

2. **Carbohydrate Metabolism**
   - Glycolysis and gluconeogenesis  
       - *Lehninger*  
   - Pentose phosphate pathway  
       - *Lehninger*  

3. **Metabolic Regulation**
   - Allosteric control and hormonal regulation  
       - *Lehninger*  
       - *Hammes*  

4. **Citric Acid Cycle**
   - Reactions, energy yield, and regulation  
       - *Lehninger*  
   - Anaplerotic and amphibolic roles  
       - *Lehninger*  

5. **Lipid Metabolism**
   - Fatty acid oxidation and ketone bodies  
       - *Lehninger*  
   - Lipid biosynthesis and regulation  
       - *Lehninger*  

6. **Amino Acid Metabolism**
   - Catabolism and nitrogen disposal (urea cycle)  
       - *Lehninger*  
   - Biosynthesis of amino acids  
       - *Lehninger*  

7. **Oxidative Phosphorylation and Photophosphorylation**
   - Electron transport chains and chemiosmosis  
       - *Lehninger*  
       - *Nicholls & Ferguson – Bioenergetics*  
   - Overlap: Proton-motive force and ΔμH+ (*Hammes*)  

8. **Integration of Metabolism**
   - Tissue-specific pathways and hormonal control  
       - *Lehninger*  

---

## **IV. Information Pathways**
1. **Genes and Chromosomes**
   - DNA structure and chromatin organization  
       - *Lehninger*  

2. **DNA Metabolism**
   - Replication, repair, and recombination  
       - *Lehninger*  
       - *Watson – Molecular Biology of the Gene*  

3. **RNA Metabolism**
   - Transcription and RNA processing  
       - *Lehninger*  

4. **Protein Metabolism**
   - Translation and post-translational modifications  
       - *Lehninger*  

5. **Regulation of Gene Expression**
   - Prokaryotic and eukaryotic systems  
       - *Lehninger*  
       - *Alberts – Molecular Biology of the Cell*  

---

### **Key Overlap Points**
- **Physical Chemistry**: Thermodynamics (ΔG, ΔH), electrochemistry (Nernst), kinetics  
- **Cell Biology**: Membranes, organelles, signal transduction, cytoskeletal motors  
- **Analytical Chemistry**: Spectroscopy, calorimetry, chromatography in biomolecule study  

---
