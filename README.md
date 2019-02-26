# Mob_Building_Occ_Energy_Use

This repository contains data and scripts that accompany the paper 

## "Planning for sustainable cities by estimating building occupancy with mobile phones"
Edward Barbour, Carlos Cerezo Davila, Siddharth Gupta, Christoph Reinhart, Jasleen Kaur, Marta C. Gonzalez

The scripts are contained with the two folders "Stay_Assignment_Scripts" and "EPS_Scripts".

To run the occupancy assignment and energyplus simulations, first go to the directory "Stay_Assignment_Scripts".
Then run the ipython notebook files:
1. Step_1_BuildingsTractArea.ipynb
2. Step_3_PickleData.ipynb
3. Step_4_POIsTractsMine.ipynb 
4. Step_5_HyperlocalBuildings.ipynb
5. Step_6_BuildingOccupancy.ipynb

The POIs don't actually need to be included since all the buildings are already classified by type. If you want to rerun this part of the analysis I have left roughly the code we used and you'll need to go through it (add your own api key etc etc).

Originally, there was a step 2 but this was removed.

During the running process a lot more files will be created in the various subdirectories

INPUT DATA:
There are two sets of input data required to run the repository in full.
These are:
1) stay points generated from the TimeGeo model of Jiang et al. (https://www.pnas.org/content/113/37/E5370.short) and the Boston buildings data (including shapefiles, per capita areas and census tract outlines). Further information about the TimeGeo model should be obtained by contacting Prof Gonzalez.
2) the idf files generated from the Sustainable design lab at MIT (by Carlos Cerezo and Christoph Reinhart). Further information about the EnergyPlus model should be obtained by contacting Prof Reinhart.

At the minute, all the data for 1 census tract is included.

To run the EnergyPlus analysis, you need EnergyPlus (https://energyplus.net/installation-linux) and Eppy (https://pythonhosted.org/eppy/runningeplus.html).

The input idf files for one tract are included in the directory "Full_idf_files". Unzip this and add the files to this directory.

In particular, you need to make sure that the path to the 'iddFile' ('Energy+.idd') is set and then to run the simulations you need EnergyPlus installed.

After the ipython notebook files have been run in the directory "Stay_Assignment_Scripts", then the scripts in the directory "EPS_Scripts" can be run.
the running order is:
1. _1_Occupancy_sensitivity_analysis.ipynb
2. _2_model_occupancy_idfs.ipynb
3. _3_energy_efficiency_apartments.ipynb
4. _4_equipment_upgrade_office.ipynb
5. _5_Running_EPlus.ipynb
6. _Results_Analysis.ipynb



