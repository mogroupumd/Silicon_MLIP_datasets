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
|&emsp;|-- DFT_K4  
|&emsp;|-- DFT_K2 (testing sets only)  
|&emsp;|-- DFT_K1 (testing sets only)  
|  
|-- Energies  
|&emsp;|-- DFT_K4  
|&emsp;|-- DFT_K2 (testing sets only)  
|  
|-- Structures: [index].POSCAR.vasp  
|  
|-- r: distances to migrating atoms (testing sets only)  
|  
|-- r_v: distances to vacancies (testing sets only)  
|  
|-- Vacancies: [index]_vacancies.POSCAR.vasp  
&emsp;&emsp;(identified vacancy sites)  
&emsp;&emsp;(testing sets only)  

# Citation
If you use the datasets extensively, you may want to cite the following publication:


# Note
The Original_Training_Set is obtained from:  
Zuo Yunxing, Chi Chen, Xiangguo Li, Zhi Deng, Yiming Chen, Jörg Behler, Gábor Csányi, et al. 2020. “Performance and Cost Assessment of Machine Learning Interatomic Potentials.” Journal of Physical Chemistry A 124 (4): 731–45. https://doi.org/10.1021/acs.jpca.9b08723.
