# ForceFields
 A repository to hold my personal developed forcefields for molecular mechanics calculations

This force field is built by combining the main parameters from `DREIDING` force field for light elements, such as C, N, H, O, and others, and parameters from `UFF` for heavy elements, both used for frameworks atoms. 

For the adsorbate atoms the parameters is taken from different sources, all documented in the `force_field_mixing_rules.def` file.

The Lennard-Jones potential has it minumum at a ditance R0 = 2^(1/6) . σ, so the conversion from R0 to sigma is made dividing R0 by 2^(1/6).
The conversion from kcal/mol to K is made dividing by the Boltzman constant (kb) in kcal/(mol.K) 0.0019872041

## DREIDING Parameters

| Atom | R0 (A)  | D0 (kcal/mol) | σ (A)   | ε (K)      |
|------|---------|---------------|---------|------------|
| H    | 3.19500 | 0.01520       | 2.84642 | 7.648938   |
| B    | 4.02000 | 0.09500       | 3.58141 | 47.805859  |
| C    | 3.89830 | 0.09510       | 3.47299 | 47.856181  |
| N    | 3.66210 | 0.07740       | 3.26256 | 38.949195  |
| O    | 3.40460 | 0.09570       | 3.03315 | 48.158113  |
| F    | 3.47200 | 0.07250       | 3.09320 | 36.483419  |
| Al   | 4.39000 | 0.31000       | 3.91105 | 155.998068 |
| Si   | 4.27000 | 0.31000       | 3.80414 | 155.998068 |
| P    | 4.15000 | 0.32000       | 3.69723 | 161.030264 |
| S    | 4.03000 | 0.34400       | 3.59032 | 173.107533 |
| Cl   | 3.95030 | 0.28330       | 3.51932 | 142.562105 |
| Ga   | 4.39000 | 0.40000       | 3.91105 | 201.287829 |
| Ge   | 4.27000 | 0.40000       | 3.80414 | 201.287829 |
| As   | 4.15000 | 0.41000       | 3.69723 | 206.320025 |
| Se   | 4.03000 | 0.43000       | 3.59032 | 216.384417 |
| Br   | 3.95000 | 0.37000       | 3.51905 | 186.191242 |
| In   | 4.59000 | 0.55000       | 4.08923 | 276.770766 |
| Sn   | 4.47000 | 0.55000       | 3.98232 | 276.770766 |
| Sb   | 4.35000 | 0.55000       | 3.87541 | 276.770766 |
| Te   | 4.23000 | 0.57000       | 3.76850 | 286.835157 |
| I    | 4.15000 | 0.51000       | 3.69723 | 256.641983 |

## UFF Parameters

| Atom | R0 (A)  | D0 (kcal/mol) | σ (A)   | ε (K)     |
|------|---------|---------------|---------|-----------|
| C    | 3.85117 | 0.10492       | 3.43100 | 52.80000  |
| O    | 3.49984 | 0.06001       | 3.11800 | 30.20000  |
| H    | 2.88585 | 0.04399       | 2.57100 | 22.14000  |
| N    | 3.66035 | 0.06895       | 3.26100 | 34.70000  |
| F    | 3.36402 | 0.04996       | 2.99700 | 25.14000  |
| Na   | 2.98350 | 0.02999       | 2.65800 | 15.09000  |
| Mg   | 3.02055 | 0.11092       | 2.69100 | 55.82000  |
| Al   | 4.49883 | 0.50460       | 4.00800 | 253.94000 |
| Si   | 4.29454 | 0.40169       | 3.82600 | 202.15000 |
| P    | 4.14750 | 0.30476       | 3.69500 | 153.37000 |
| S    | 4.03525 | 0.27378       | 3.59500 | 137.78000 |
| Cl   | 3.94658 | 0.22683       | 3.51600 | 114.15000 |
| K    | 3.81188 | 0.03497       | 3.39600 | 17.60000  |
| Ca   | 3.39882 | 0.23782       | 3.02800 | 119.68000 |
| Sc   | 3.29555 | 0.01898       | 2.93600 | 9.55000   |
| Ti   | 3.17545 | 0.01699       | 2.82900 | 8.55000   |
| V    | 3.14402 | 0.01600       | 2.80100 | 8.05000   |
| Cr   | 3.02279 | 0.01498       | 2.69300 | 7.54000   |
| Mn   | 2.96105 | 0.01300       | 2.63800 | 6.54000   |
| Fe   | 2.91167 | 0.01300       | 2.59400 | 6.54000   |
| Co   | 2.87238 | 0.01399       | 2.55900 | 7.04000   |
| Ni   | 2.83422 | 0.01498       | 2.52500 | 7.54000   |
| Cu   | 3.49535 | 0.00499       | 3.11400 | 2.51000   |
| Zn   | 2.76350 | 0.12395       | 2.46200 | 62.38000  |
| Zr   | 3.12381 | 0.06895       | 2.78300 | 34.70000  |
| Mo   | 3.05197 | 0.05596       | 2.71900 | 28.16000  |
| Re   | 2.95432 | 0.06595       | 2.63200 | 33.19000  |
| Be   | 2.74554 | 0.08493       | 2.44600 | 42.74000  |
| B    | 4.08352 | 0.17985       | 3.63800 | 90.51000  |
| Zn   | 2.76350 | 0.12390       | 2.46200 | 62.35000  |
| Ga   | 4.38321 | 0.41469       | 3.90500 | 208.69000 |
| Ge   | 4.27995 | 0.37870       | 3.81300 | 190.58000 |
| As   | 4.23056 | 0.30875       | 3.76900 | 155.38000 |
| Se   | 4.20474 | 0.29077       | 3.74600 | 146.33000 |
| Br   | 4.18903 | 0.25081       | 3.73200 | 126.22000 |
| Rb   | 4.11382 | 0.03996       | 3.66500 | 20.11000  |
| Sr   | 3.64127 | 0.23481       | 3.24400 | 118.17000 |
| Y    | 3.34494 | 0.07195       | 2.98000 | 36.21000  |
| Nb   | 3.16534 | 0.05896       | 2.82000 | 29.67000  |
| Tc   | 2.99810 | 0.04797       | 2.67100 | 24.14000  |
| Ru   | 2.96330 | 0.05596       | 2.64000 | 28.16000  |
| Rh   | 2.92850 | 0.05296       | 2.60900 | 26.65000  |
| Pd   | 2.89932 | 0.04797       | 2.58300 | 24.14000  |
| Ag   | 3.14851 | 0.03597       | 2.80500 | 18.10000  |
| Cd   | 2.84769 | 0.22782       | 2.53700 | 114.65000 |
| In   | 4.46291 | 0.59853       | 3.97600 | 301.21000 |
| Sn   | 4.39219 | 0.56656       | 3.91300 | 285.12000 |
| Sb   | 4.42026 | 0.44865       | 3.93800 | 225.78000 |
| Te   | 4.46964 | 0.39770       | 3.98200 | 200.14000 |
| Cs   | 4.51679 | 0.04497       | 4.02400 | 22.63000  |
| Ba   | 3.70300 | 0.36372       | 3.29900 | 183.04000 |
| La   | 3.52229 | 0.01699       | 3.13800 | 8.55000   |
| Ce   | 3.55596 | 0.01300       | 3.16800 | 6.54000   |
| Pr   | 3.60647 | 0.01000       | 3.21300 | 5.03000   |
| Nd   | 3.57504 | 0.01000       | 3.18500 | 5.03000   |
| Pm   | 3.54698 | 0.00900       | 3.16000 | 4.53000   |
| Sm   | 3.52004 | 0.00799       | 3.13600 | 4.02000   |
| Eu   | 3.49310 | 0.00799       | 3.11200 | 4.02000   |
| Gd   | 3.36851 | 0.00900       | 3.00100 | 4.53000   |
| Tb   | 3.45045 | 0.00699       | 3.07400 | 3.52000   |
| Dy   | 3.42800 | 0.00699       | 3.05400 | 3.52000   |
| Ho   | 3.40892 | 0.00699       | 3.03700 | 3.52000   |
| Er   | 3.39096 | 0.00699       | 3.02100 | 3.52000   |
| Tm   | 3.37412 | 0.00600       | 3.00600 | 3.02000   |
| Yb   | 3.35504 | 0.22782       | 2.98900 | 114.65000 |
| Lu   | 3.64014 | 0.04097       | 3.24300 | 20.62000  |
| Hf   | 3.14065 | 0.07195       | 2.79800 | 36.21000  |
| Ta   | 3.16983 | 0.08093       | 2.82400 | 40.73000  |
| W    | 3.06881 | 0.06695       | 2.73400 | 33.69000  |
| Re   | 2.95432 | 0.06595       | 2.63200 | 33.19000  |
| Os   | 3.12044 | 0.03698       | 2.78000 | 18.61000  |
| Ir   | 2.83983 | 0.07295       | 2.53000 | 36.71000  |
| Pt   | 2.75452 | 0.07994       | 2.45400 | 40.23000  |
| Au   | 3.29330 | 0.03897       | 2.93400 | 19.61000  |
| Hg   | 2.70513 | 0.38470       | 2.41000 | 193.60000 |
| Tl   | 4.34730 | 0.67947       | 3.87300 | 341.94000 |
| Pb   | 4.29678 | 0.66248       | 3.82800 | 333.39000 |
| Bi   | 4.36974 | 0.51760       | 3.89300 | 260.48000 |
| Po   | 4.70873 | 0.32475       | 4.19500 | 163.43000 |
| At   | 4.75026 | 0.28378       | 4.23200 | 142.81000 |
| Rn   | 4.76485 | 0.24781       | 4.24500 | 124.71000 |
| Ra   | 3.67719 | 0.40368       | 3.27600 | 203.15000 |
| Ac   | 3.47851 | 0.03297       | 3.09900 | 16.59000  |
| Th   | 3.39545 | 0.02597       | 3.02500 | 13.07000  |
| Pa   | 3.42351 | 0.02198       | 3.05000 | 11.06000  |
| U    | 3.39545 | 0.02198       | 3.02500 | 11.06000  |
| Np   | 3.42351 | 0.01898       | 3.05000 | 9.55000   |
| Pu   | 3.42351 | 0.01600       | 3.05000 | 8.05000   |
| Am   | 3.38086 | 0.01399       | 3.01200 | 7.04000   |
| Cm   | 3.32586 | 0.01300       | 2.96300 | 6.54000   |
| Bk   | 3.33932 | 0.01300       | 2.97500 | 6.54000   |
| Cf   | 3.31351 | 0.01300       | 2.95200 | 6.54000   |
| Es   | 3.29892 | 0.01198       | 2.93900 | 6.03000   |
| Fm   | 3.28545 | 0.01198       | 2.92700 | 6.03000   |
| Md   | 3.27422 | 0.01099       | 2.91700 | 5.53000   |
| No   | 3.24841 | 0.01099       | 2.89400 | 5.53000   |
| Lw   | 3.23606 | 0.01099       | 2.88300 | 5.53000   |

## Instalation 

To install this force field you can create a new folder on the compiled raspa forcefield directory, usually on the folder: `${RASPA_DIR}/share/raspa/forcefield/`, and put the tree files in the `DREIDING-UFF-TRAPPE` on this new folder. You can put any name that you want, just remember to put this same name on the script to run the RASPA simulation under the `Forcefield` variable tag. 

You can also just put these tree files on the folder that you are running the RASPA, with the variable `Local` as the force field. The program always search for force field files on the local folder first. 

Finally, you can put the folder `Trappe` on the `${RASPA_DIR}/share/raspa/molecules/` directory. This folder contains the molecule definitions (i.e. atomic type, positions and thermodynamic informations) for the program to run the simmulations. These informations are taken from the [TraPPE](http://trappe.oit.umn.edu/) database. 
