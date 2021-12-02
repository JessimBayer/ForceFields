# Force Fields
 A repository to hold my personal developed forcefields for molecular mechanics calculations

This force field is built by combining the main parameters from `DREIDING` force field for light elements, such as C, N, H, O, and others, and parameters from `UFF` for heavy elements, both used for frameworks atoms. 

For the adsorbate atoms the parameters is taken from different sources, all documented in the `force_field_mixing_rules.def` file.

<img src="https://user-images.githubusercontent.com/33868364/144495503-e21b139e-a3ee-4ba7-af54-3df163ce9fcf.png" alt="Schematic_of_the_Lennard-Jones_6-12_Potential" width="400"/>

![CodeCogsEqn](https://user-images.githubusercontent.com/33868364/144495206-9dd075db-1c04-4969-98fc-3cb84b82e332.png)


The Lennard-Jones potential has it minumum at a ditance R<sub>min</sub> = 2<sup>1/6</sup> . σ, so the conversion from R<sub>min</sub> to sigma is made dividing R<sub>min</sub> by 2<sup>1/6</sup>.

The conversion from kcal/mol to K is made dividing by the Boltzman constant (K<sub>b</sub>) in kcal/[mol.K] = 0.0019872041

## DREIDING Parameters

Parameters taken from Table II of *MAYO, Stephen L.; OLAFSON, Barry D.; GODDARD, William A. DREIDING: a generic force field for molecular simulations. Journal of Physical chemistry, v. 94, n. 26, p. 8897-8909, 1990.*

| Atom | R<sub>min</sub> (A)  | D<sub>0</sub> (kcal/mol) | σ (A)   | ε (K)      |
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

Parameters taken from Table 1 of *RAPPÉ, Anthony K. et al. UFF, a full periodic table force field for molecular mechanics and molecular dynamics simulations. Journal of the American chemical society, v. 114, n. 25, p. 10024-10035, 1992.*

| Atom | R<sub>min</sub> (A)  | D<sub>0</sub> (kcal/mol) | σ (A)    | ε (K)     |
|------|----------|---------------|----------|-----------|
| C    | 3.85100  | 0.10500       | 3.43085  | 52.83806  |
| O    | 3.50000  | 0.06000       | 3.11815  | 30.19317  |
| H    | 2.88600  | 0.04400       | 2.57113  | 22.14166  |
| N    | 3.66000  | 0.06900       | 3.26069  | 34.72215  |
| F    | 3.36400  | 0.05000       | 2.99698  | 25.16098  |
| Na   | 2.98300  | 0.03000       | 2.65755  | 15.09659  |
| Mg   | 3.02100  | 0.11100       | 2.69141  | 55.85737  |
| Al   | 4.49900  | 0.50500       | 4.00815  | 254.12588 |
| Si   | 4.29500  | 0.40200       | 3.82641  | 202.29427 |
| P    | 4.14700  | 0.30500       | 3.69456  | 153.48197 |
| S    | 4.03500  | 0.27400       | 3.59478  | 137.88216 |
| Cl   | 3.94700  | 0.22700       | 3.51638  | 114.23084 |
| K    | 3.81200  | 0.03500       | 3.39611  | 17.61269  |
| Ca   | 3.39900  | 0.23800       | 3.02816  | 119.76626 |
| Sc   | 3.29500  | 0.01900       | 2.93551  | 9.56117   |
| Ti   | 3.17500  | 0.01700       | 2.82860  | 8.55473   |
| V    | 3.14400  | 0.01600       | 2.80099  | 8.05151   |
| Cr   | 30.23000 | 0.01500       | 26.93187 | 7.54829   |
| Mn   | 2.96100  | 0.01300       | 2.63795  | 6.54185   |
| Fe   | 2.91200  | 0.01300       | 2.59430  | 6.54185   |
| Co   | 2.87200  | 0.01400       | 2.55866  | 7.04507   |
| Ni   | 2.83400  | 0.01500       | 2.52481  | 7.54829   |
| Cu   | 3.49500  | 0.00500       | 3.11369  | 2.51610   |
| Zn   | 2.76300  | 0.12400       | 2.46155  | 62.39923  |
| Zr   | 3.12400  | 0.06900       | 2.78317  | 34.72215  |
| Mo   | 3.05200  | 0.05900       | 2.71902  | 29.68995  |
| Be   | 2.74500  | 0.08500       | 2.44552  | 42.77366  |
| B    | 4.08300  | 0.18000       | 3.63754  | 90.57952  |
| Ga   | 4.38300  | 0.41500       | 3.90481  | 208.83612 |
| Ge   | 4.28000  | 0.37900       | 3.81305  | 190.72022 |
| As   | 4.23000  | 0.30900       | 3.76850  | 155.49485 |
| Se   | 4.20500  | 0.29100       | 3.74623  | 146.43690 |
| Br   | 4.18900  | 0.25100       | 3.73197  | 126.30811 |
| Rb   | 4.11400  | 0.04000       | 3.66516  | 20.12878  |
| Sr   | 3.64100  | 0.23500       | 3.24376  | 118.25660 |
| Y    | 3.34500  | 0.07200       | 2.98006  | 36.23181  |
| Nb   | 3.16500  | 0.05900       | 2.81969  | 29.68995  |
| Tc   | 2.99800  | 0.04800       | 2.67091  | 24.15454  |
| Ru   | 2.96300  | 0.05600       | 2.63973  | 28.18030  |
| Rh   | 2.92900  | 0.05300       | 2.60944  | 26.67064  |
| Pd   | 2.89900  | 0.04800       | 2.58272  | 24.15454  |
| Ag   | 3.14800  | 0.03600       | 2.80455  | 18.11590  |
| Cd   | 2.84800  | 0.22800       | 2.53728  | 114.73406 |
| In   | 4.46300  | 0.59900       | 3.97608  | 301.42852 |
| Sn   | 4.39200  | 0.56700       | 3.91283  | 285.32550 |
| Sb   | 4.42000  | 0.44900       | 3.93777  | 225.94559 |
| Te   | 4.47000  | 0.39800       | 3.98232  | 200.28139 |
| Cs   | 4.51700  | 0.04500       | 4.02419  | 22.64488  |
| Ba   | 3.70300  | 0.36400       | 3.29900  | 183.17192 |
| La   | 3.52200  | 0.01700       | 3.13775  | 8.55473   |
| Ce   | 3.55600  | 0.01300       | 3.16804  | 6.54185   |
| Pr   | 3.60600  | 0.01000       | 3.21258  | 5.03220   |
| Nd   | 3.57500  | 0.01000       | 3.18496  | 5.03220   |
| Pm   | 3.54700  | 0.00900       | 3.16002  | 4.52898   |
| Sm   | 3.52000  | 0.00800       | 3.13596  | 4.02576   |
| Eu   | 3.49300  | 0.00800       | 3.11191  | 4.02576   |
| Gd   | 3.36800  | 0.00900       | 3.00055  | 4.52898   |
| Tb   | 3.45100  | 0.00700       | 3.07449  | 3.52254   |
| Dy   | 3.42800  | 0.00700       | 3.05400  | 3.52254   |
| Ho   | 3.40900  | 0.00700       | 3.03707  | 3.52254   |
| Er   | 3.39100  | 0.00700       | 3.02104  | 3.52254   |
| Tm   | 3.37400  | 0.00600       | 3.00589  | 3.01932   |
| Yb   | 3.35500  | 0.22800       | 2.98897  | 114.73406 |
| Lu   | 3.64000  | 0.04100       | 3.24287  | 20.63200  |
| Hf   | 3.14100  | 0.07200       | 2.79831  | 36.23181  |
| Ta   | 3.17000  | 0.08100       | 2.82415  | 40.76079  |
| W    | 3.06900  | 0.06700       | 2.73417  | 33.71571  |
| Re   | 2.95400  | 0.06600       | 2.63171  | 33.21249  |
| Os   | 3.12000  | 0.03700       | 2.77960  | 18.61912  |
| Ir   | 2.84000  | 0.07300       | 2.53015  | 36.73503  |
| Pt   | 2.75400  | 0.08000       | 2.45354  | 40.25757  |
| Au   | 3.29300  | 0.03900       | 2.93373  | 19.62556  |
| Hg   | 2.70500  | 0.38500       | 2.40988  | 193.73954 |
| Tl   | 4.34700  | 0.68000       | 3.87274  | 342.18931 |
| Pb   | 4.29700  | 0.66300       | 3.82819  | 333.63458 |
| Bi   | 4.37000  | 0.51800       | 3.89323  | 260.66774 |
| Po   | 4.70900  | 0.32500       | 4.19524  | 163.54636 |
| At   | 4.75000  | 0.28400       | 4.23177  | 142.91436 |
| Rn   | 4.76500  | 0.24800       | 4.24513  | 124.79845 |
| Ra   | 3.67700  | 0.40400       | 3.27583  | 203.30071 |
| Ac   | 3.47800  | 0.03300       | 3.09855  | 16.60625  |
| Th   | 3.39600  | 0.02600       | 3.02549  | 13.08371  |
| Pa   | 3.42400  | 0.02200       | 3.05044  | 11.07083  |
| U    | 3.39500  | 0.02200       | 3.02460  | 11.07083  |
| Np   | 3.42400  | 0.01900       | 3.05044  | 9.56117   |
| Pu   | 3.42400  | 0.01600       | 3.05044  | 8.05151   |
| Am   | 3.38100  | 0.01400       | 3.01213  | 7.04507   |
| Cm   | 3.32600  | 0.01300       | 2.96313  | 6.54185   |
| Bk   | 3.33900  | 0.01300       | 2.97471  | 6.54185   |
| Cf   | 3.31300  | 0.01300       | 2.95155  | 6.54185   |
| Es   | 3.29900  | 0.01200       | 2.93907  | 6.03863   |
| Fm   | 3.28600  | 0.01200       | 2.92749  | 6.03863   |
| Md   | 3.27400  | 0.01100       | 2.91680  | 5.53542   |
| No   | 3.24800  | 0.01100       | 2.89364  | 5.53542   |
| Lw   | 3.23600  | 0.01100       | 2.88295  | 5.53542   |


## Instalation 

To install this force field you can create a new folder on the compiled raspa forcefield directory, usually on the folder: `${RASPA_DIR}/share/raspa/forcefield/`, and put the tree files in the `DREIDING-UFF-TRAPPE` on this new folder. You can put any name that you want, just remember to put this same name on the script to run the RASPA simulation under the `Forcefield` variable tag. 

You can also just put these tree files on the folder that you are running the RASPA, with the variable `Local` as the force field. The program always search for force field files on the local folder first. 

Finally, you can put the folder `Trappe` on the `${RASPA_DIR}/share/raspa/molecules/` directory. This folder contains the molecule definitions (i.e. atomic type, positions and thermodynamic informations) for the program to run the simmulations. These informations are taken from the [TraPPE](http://trappe.oit.umn.edu/) database. 
