# NEP_potentials
The machine learning NEP potentials for different materials generated and used in our group.

Available NEP potentials include:
1. AgCrSe2: train / test datasets (a supercell of 216 atoms) calculated by VASP with PBE XC functionals. The ground-state of AgCrSe2 is assumed to be ferromagnetic. It's recommended that D3 is included at the NEP+D3 level, which results in very good lattice parameters at RT. Note that the configurations used for training is quite small. But it can successfully pass a very long MD run (~10 ns) at 700 K.
2. BaTiS3: train / test datasets (a supercell of xxx atoms) calculated by VASP with HSE06 XC functionals. We have also tested PBE and r2SCAN+rvv10 XC functionals agains HSE06. But only HSE06 results in correct semiconducting ground-state with a small band-gap. This is very possibly due to the strong charge-transfer between Ti and S atoms. Note that the configurations used for training is quite small because of the really heavy computational cost of HSE06.
