# QM-22
Datasets of molecules many of which "certified" for diffusion Monte Carlo calculations of the zero-point state, except as noted.  Here are
the citations for each dataset.  Details of how the datasets were generated are molecule-specific and are given in these
papers.  

**Data File Format**

Number of atoms  
Energy (hartree)  
Atom label and cartesian coords (angstrom) gradient components if included  (hartree/bohr)”


**n-tetradecane C<sub>14</sub>H<sub>30</sub>**

B3LYP energies and gradients, not DMC certified

“DFT-Based Permutationally Invariant Polynomial Potentials Capture the Twists and Turns of C<sub>14</sub>H<sub>30</sub>”, Qu, et al. (in preparation)

**NaCl-H<sub>2</sub> interaction**

CCSD(T)/aug-cc-pVTZ energies. These are interaction energies (that is, E<sub>int</sub> = E<sub>dimer</sub> - E<sub>NaCl</sub> - E<sub>hydrogen</sub>

“Ab Initio Potential Energy Surface for NaCl−H<sub>2</sub> with Correct Long-Range Behavior”, Pandey, et al., J. Phys. Chem. A 128, 902 (2024)

**Acetaldehyde (singlet)**

CCSD(T) and MRCI energies

“Quasiclassical trajectory calculations of the dissociation dynamics of CH<sub>3</sub>CHO at high energy yield many products”, Han, et al., J. Phys. Chem. Lett. 2, 1715 (2011).
“Photodissociation of CH<sub>3</sub>CHO at 248 nm: identification of the channels of roaming, triple fragmentation and the transition state”, Han, et al., Phys. Chem. Chem. Phys. 19, 18628 (2017).

**Acetaldehyde (triplet)**

CCSD(T) energies

“Intersystem crossing and dynamics in O(<sup>3</sup>P)+C<sub>2</sub>H<sub>4</sub> multichannel reaction: Experiment validates theory”, Fu, et al., Proc. Nat. Acad. Sci. 109, 9733 (2012).

**Ethanol**

B3LYP energies and gradients

“Permutationally invariant polynomial regression for energies and gradients using backward differentiation achieves orders of magnitude speed-up while keeping high precision compared to other machine learning methods”, Houston et al. J. Chem. Phys. 156, 044120 (2022)

**Glycine**

B3LYP energies and gradients

“Full-dimensional, ab initio potential energy surface for glycine with characterization of stationary points and zero-point energy calculations by means of diffusion Monte Carlo and semiclassical dynamics“, Conte et al.,  J. Chem. Phys. 153, 244301 (2020)

**Malonaldehyde**

CCSD(T)/CBS energies

“Full-dimensional quantum calculations of ground-state tunneling splitting of malonaldehyde using an accurate ab initio potential energy surface”, Wang et al., J. Chem. Phys. 128, 224314 (2008)

**Methane**

B3LYP energies and gradients

“Using Gradients in Permutationally Invariant Polynomial Potential Fitting: A Demonstration for CH<sub>4</sub> Using as Few as 100 Configurations”, Nandi et al.  J. Chem. Theory Comput. 2019, 15, 2826−2835

**syn-CH<sub>3</sub>CHOO**

CCSD(T)/MRCI energies only

“Unimolecular dissociation dynamics of vibrationally activated CH<sub>3</sub>CHOO Criegee intermediates to OH radical products”, Kidwell et al, Nat. Chem. 8, 509–514 (2016)

**Tropolone**

B3LYP energies and gradients

“Permutationally Invariant Polynomial Potential Energy Surfaces for Tropolone and H atom Tunneling Dynamics”,Houston et al, J. Chem. Phys. 153 024107 (2020).

**N-methyl acetamide**

B3LYP energies and gradients

“Full and fragmented permutationally invariant polynomial potential energy surfaces for transand cis N-methyl acetamide and isomerization saddle points”, Nandi et al, J. Chem. Phys. 151, 084306 (2019).

**Hydronium H<sub>3</sub>O<sup>+</sup>, OCHCO<sup>+</sup>, H<sub>2</sub>CO/cis-trans HCOH, formic acid dimer**

CCSD(T) or MRCI energies only

“Assessing Gaussian Process Regression and Permutationally Invariant Polynomial Approaches To Represent High-Dimensional Potential Energy Surfaces” Qu et at. J. Chem.Theory Comput.14, 3381 (2018)

**Hydroxide Hydrate H<sub>3</sub>O<sub>2</sub><sup>-</sup>**

H3O2M @ 6dade4a submodule is linked to a GitHub repository with sGDML potential and the corresponding dataset for Hydroxide Hydrate. 

The dataset was described and first reported in Mrinal Arandhara and Sai G. Ramesh “Nuclear Quantum Effects in Hydroxide Hydrate Along the H-Bond Bifurcation Pathway”. J. Phys. Chem. A 2024, 128, 1600-1610.

It was subsequently used in Priyanka Pandey, Mrinal Arandhara, Paul L. Houston, Chen Qu, Riccardo Conte, Joel M. Bowman, and Sai G. Ramesh, “Assessing Permutationally Invariant Polynomial and Symmetric Gradient Domain Machine Learning Potential Energy Surfaces for H3O2-” J. Phys. Chem. A 2024, 128, 3212–3219

**Zundel H<sub>5</sub>O<sub>2</sub><sup>+</sup>**

The dataset was first reported in Xinchuan Huang, Bastiaan J. Braams, Jeol M. Bowman, “Ab initio potential energy and dipole moment surfaces for H5O2+”, J. Chem. Phys. 2005, 122, 044308

**Summary**

| Molecule | N<sub>points</sub> | Energies | Gradients |
| -------- | -----------------: | -------: | :-------: |
| n-tetradecane                        | 253,646 | B3LYP        | Yes |
| NaCl-H<sub>2</sub>                   | 281,031 | CCSD(T)      |  No |
| Acetaldehyde (singlet)               | 202,518 | CCSD(T)/MRCI |  No |
| Acetaldehyde (triplet)               |  51,530 | CCSD(T)      |  No |
| Ethanol                              |  11,011 | B3LYP        | Yes |
| Formic acid dimer                    |  13,475 | CCSD(T)      |  No |
| Glycine                              |  70,099 | B3LYP        | Yes |
| H<sub>2</sub>CO, cis- and trans-HCOH |  34,750 | MRCI         |  No |
| Hydronium                            |  32,141 | CCSD(T)      |  No |
| Malonaldehyde                        |  11,145 | CCSD(T)      |  No |
| Methane                              |   9,000 | B3LYP        | Yes |
| N-methyl acetamide                   |   6,607 | B3LYP        | Yes |
| OCHCO<sup>+</sup>                    |   7,800 | CCSD(T)      |  No |
| Tropolone                            |   6,768 | B3LYP        | Yes |
| syn-CH<sub>3</sub>CHOO               | 159,474 | CCSD(T)/MRCI |  No |
| Zundel                               |  48,149 | CCSD(T)      |  No |
