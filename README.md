# AutoRunWRFChem CBMZ(chem_opt=170) IRR + IPR with nudging for 4.1.5
scripts for running CBMZ (chem_opt = 170) WRF-Chem 4.1.5
auto create namelist for real.exe and wrf.exe

Codes in WRF-Chem (4.1.5) have been modified for outputting IRR from KPP CBMZ_8bin (chem_opt=170).
This version of WRF-Chem can also output more IPR species.


# To Run: 
source 01_envVar_set.sh
source ~/.bash_profile
bash 02_realnoChem.sh && bash 03_megan.sh && bash 04_realChem.sh && bash 05_mozbc.sh
