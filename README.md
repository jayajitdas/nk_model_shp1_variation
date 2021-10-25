# nk_model_shp1_variation
The .rxn file contains the code written using Stochastic Simulation Complier (SSC). SSC is freely availble for download from 
http://web.mit.edu/irc/ssc/. The .rxn (e.g., test_f.rxn) file is complied using SSC as, 
prompt> ssc test_f.rxn <enter> 
which creates an executable file test_f. The executable test_f is run using the input parameters contained in the .cfg file (e.g., param.cfg) 
to generate the output data. 

The file nksig_S6.rxn is used to generate the signaling kinetics for CD16 (nksig_S6_CD16.cfg) and NKp46 (nksig_S6_nkp46.cfg) stimulations. The file nksig_S6.rxn 
contains the same reactions used in Das J, Biophysical Journal (2010) PMID: 20923636 with added reactions pErk + S6 <-> pErk-S6 -> pS6 -> S6 in the signaling network. The number of inhibitory ligands in the .cfg files are set to zero, so that the inhibitory receptors are not stimulated.  The SHP-1 and CD16/NKp46 ligand concentrations are varied as shown in figures 2C and 2D. Those variations are carried out by the variables denalig (for CD16/NKp46) and denshp (for SHP1) in the .cfg files using shell scripts.  
