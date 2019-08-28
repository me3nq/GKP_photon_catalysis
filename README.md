# GKP_photon_catalysis
Series of Python codes written with the Jupyter Notebook to simulate photon catalysis and generate various non-Gaussian quantum states.  The results of this work are available on ArXiv in the paper "Gottesman-Kitaev-Preskill state preparation by photon catalysis" arXiv:1903.01925v2. 

A brief discription of the codes can be found below:

"Functions for Quantum Optics" - defines and describes the different functions that are used to define different quantum states and the operations used in the simulations.

"Single photon displacement with loss" - Contains the calculations used for Sec. III (Exact Displaced Single-Photon States) of the associated ArXiv article.  The function to perform photon catalysis is used to generate displaced single-photon state from inputs of a coherent state and a single photon.  Detector inefficiencies are also considered, and it can be seen that modifying the initial coherent state amplitude subject to specific detection events can still result in a displaced single photon state that has a higher fidelity with the ideal case that that of the normal experimental method (more details in the article.)

"Two_step_Catalysis", "Three_step_Catalysis", and "Four_step_Catalysis" - These files simulate the evolution of the quantum state after the cascaded photon catalysis described by Eq. (16) subject to specific parameters obtained by optimizing Eq. (22).  These files were used to generate Fig. 4 in Sec IV.

"Detection Efficiency effects" and "Impure Single Photon Input" - These files are relatively self-explanatory by their titles.  They each consider the different multi-step photon catalysis processes from the previous files and now include either photon-number-resolving detectors with imperfect quantum efficiency, or by including impure single-photon inputs (specifically, mixtures of single photon and vacuum).

"SSV Breeding" - This file accompanies Section V-A and is used to generate Fig. 9.  Here, it can be seen that states of the form of Eq. (24) can undergo 'breeding' into a same-class state but with increased amplitude, according to Eq. (27).  This code is used to numerically demonstrate the initial state-amplitude needed for the breeding process to yield high-fidelity results.  It also generates the probability of success.

"Square GKP from cat states" - This code takes two states generated from the cascaded photon catalysis code and subjects them to both homodyne detection and photon-number-resolved detection after interference at a beamsplitter.  Both detection types can project the resultant states into grid-like states that resemble GKP states, however, the PNR detection seems to yield more versatile results.  These results are shown in Fig. 10 of the ArXiv paper.

"Tri_SSV_Hex_GKP" - This code takes a state with higher symmetry in phase space (Eq. 25, Fig. 8) and uses a simular protocol to the previous code to generate hexagonally symmetric states in phase-space.  Specifically, PNR detection is shown to yield the hexagonal symmetry while homodyne detection does not.  More details can be found in Section V-C and Fig. 11.

"Best_HexGKP_vs_homodyne" - This code highlights the differences between homodyne and PNR detection schemes when generation hexagonally symmetric Wigner functions in phase-space.
