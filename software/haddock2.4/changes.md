---
layout: page
tags: [Jekyll, HADDOCK, Bonvin, Docking, Simulation, Molecular Dynamics, Structural Biology, Computational Biology, Modelling, Protein Structure]
modified: 2014-08-08T20:53:07.573882-04:00
comments: false
image:
  feature: pages/banner_software.jpg
---
### Latest changes - version January 2023
- Added missing SIA-NGA 2-6 glycosilic linkages
- Added support for SIA-SIA 2-8 linkages
- Implemented automatic DNA/RNA restraints definition


### changes- version August 2022
- Added support for 3-Hydroxyproline (HY3 residue)
- Added improper to tensor topology
- Extended support for 10 RDC restraint sets
- Implemented move of RDC and DANI tensors after it1 for numerical stability


### changes - version January 2022
- Minor changes in occupancy treatment for pharmacophore-based shape docking
- Added support for 2-N-acetyl-beta-D-galactopyranose (NGA)
- Added support for N-methylated Cter (NME residue)
- Various changes to support DPP membranes
- Made glycan rings rigid for torsion angle dynamics
- Corrected issue with initialisation of contact probabilities for solvated docking
- Corrected issue when using the DNA-RNA linkage file to keep the terminal 5'phosphate
- Corrected issue with BSA calculation in the presence of tensors
- Corrected issue with Rg energy in PDB output files


### Changes - version May 2021
- Fixed issue with grid package submission for model-specific ambig files
- Added carbohydrates to scoring scripts
- Fixed clustering issue in case of single model runs
- Improvements, optimizations and fixes to the internal scheduler subroutines


### Changes - version January 2021
- Added support ASN-BGC glycosilic linkage
- Fixed an issue in which clustering would fail if complexes had too many chains
- Added an extra check for solvated docking and waterdock
- Fixed a bug where simulations would fail if too many ions were restrained
- Improvements, optimizations and fixes to the internal scheduler subroutines


### Changes - version September 2020
- Added beta sialic acid (SIB), and additional linkages between glycans
- Added modified DNA baseJ (DJ)
- Corrected issue with automatic his protonation state
- Added automatic definition of restraints to maintain ions in their coordination sphere.
- Modified analysis scripts to work with a single ligand molecule


### Changes - version July 2020
- Added support for glycosylated proteins
- Improved diagnostics
- Minor fixes and code cleaning
 

### Changes - version June 2020
- Adapted the CG-to-AA conversion script to allow to morph larger conformational changes
  and use secondary structure restraints
- Corrected an issue in automatic secondary structure definition leading failures for very large systems
- Exposed a new parameter in run.cns (flcut_nb) that allows to control the distance cutoff to automatically
  define semi-flexible regions

	
### Changes with respect to version 2.2
- Extension to up to 20 molecules docking
- Coarse grained docking implemented based on the Martini force field v2.2
  for both proteins and nucleic acids
- Z-restraining potential as implicit membrane restraining potential
- Cryo-EM restraints implementation
- Added option to turn off (partially) analysis (speeds up the overall running time)
  Default settings only perform clustering
- For refinement (randorien=false), missing atoms are now rebuilt in the context of the complex
- Added automatic identification of cyclic peptides
- Added automatic idenfification of D-amino acids
- Added support for C6 symmetry
- Added support for shapes
- Added option to automatically define HIS protonation states based on electrostatic energy
- Changed default dielectric treatment to distance dependent dielectric with eps=10 for it0 and 1 for it1
  (Note should not be used for nucleic acids and coarse graining)
- Turn off by default explicit solvent final refinement (only EM performed)
- Switched nucleic acid support to use 1/2 letter code for RNA/DNA
- Added option to fix molecules in their original position


* * *

<font size="-1">Please send any suggestions or enquiries to Alexandre Bonvin</font>
