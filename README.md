# Silicon_MLP_datasets
Training, validation, and testing datasets for the publication "The discrepancies, the extrapolability, and the interpolability of machine learning interatomic potentials on simulating atomic dynamics"

# Data architecture
Each directory contains:
1.  The compressed structural data (in VASP POSCAR format with .zip file)
2.  The corresponding energies, forces, distances to nearest migrating atoms, and distances to nearest vacancies data  (DATA.json)
3.  (Available only for testing datasets) the compressed structural data for vacancies (in VASP POSCAR format with .zip file)

DATA.json architecture:
|
|-- Forces
|       |-- DFT_K4
|       |-- DFT_K2 (testing sets only)
|       |-- DFT_K1 (testing sets only)
|
|-- Energies
|       |-- DFT_K4
|       |-- DFT_K2 (testing sets only)
|
|-- Structures: [index].POSCAR.vasp
|
|-- r: distances to migrating atoms (testing sets only)
|
|-- r_v: distances to vacancies (testing sets only)
|
|-- Vacancies: [index]_vacancies.POSCAR.vasp
               (identified vacancy sites)
               (testing sets only)

# Citation
If you use the datasets extensively, you may want to cite the following publication:
