# QM7 Quantum Chemistry Dataset

### Introduction
This dataset is the public dataset QM7 from [this](http://quantum-machine.org/datasets/) group of datasets, which includes quantum data simulated by the [FHI group](https://www.fhi.mpg.de/th-department) at the Max Planck Institute.

### Data Gathering
The QM7 dataset is a small portion of the GDB-13 dataset, containing all molecules of up to 23 atoms (including 7 heavy atoms C, N, O, and S), totalling 7165 molecules. We provide the Coulomb matrix representation of these molecules and their atomization energies computed similarly to the FHI-AIMS implementation of the Perdew-Burke-Ernzerhof hybrid functional (PBE0).

### Data Formatting
The data is split into 5 separate features (matrices) saved as numpy arrays. The 5 matrices are labelled as follows:
- X (7165 x 23 x 23) - The Coulomb matrices
- T (7165) - The atomization energies
- P (5 x 1433) - Splits for cross-validation
- Z (7165) - Atomic charge
- R (7165 x 3) - Cartesian coordinates of each atom in the molecules


### Application
This dataset is aimed to be used in the field of quantum chemistry, particularly targeting the esimation of atomization energies given the structure of chemical molecules.

