# AutoRunWRFChem CBMZ(chem_opt=170) IRR + IPR NO nudging Under PBL for 4.1.5
scripts for running CBMZ (chem_opt = 170) WRF-Chem 4.1.5
auto create namelist for real.exe and wrf.exe

Codes in WRF-Chem (4.1.5) have been modified for outputting IRR from KPP CBMZ_8bin (chem_opt=170).
This version of WRF-Chem can also output more IPR species.
# wet scavenging in stratocumulus clouds and aqueous chemistry in stratocumulus clouds are not supported in cbmz170
wetscav_onoff                       = 0
cldchem_onoff                       = 0



# To Run: 
source 01_envVar_set.sh
source ~/.bash_profile
bash 02_realnoChem.sh && bash 03_megan.sh && bash 04_realChem.sh && bash 05_mozbc.sh
