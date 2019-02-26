# Mob_Building_Occ_Energy_Use

Updating: Changing to one tract run

This repository contains data and scripts for assigning stay points to buildings to generate building occupancy profiles, and subsequently run energyplus simulations for a subset of around 1400 buildings in the city of Boston.

The scripts are contained with the two folders "Stay_Assignment_Scripts" and "EPS_Scripts".
The scripts are numbered and can be run sequentially (stay assignments must be run before EPS)

During the running process a lot more files will be created in the various subfolders

INPUT DATA:
There are two sets of input data required to run the repository in full.
These are:
1) stay points generated from the TimeGeo model of Jiang et al. [1] and the Boston buildings data (including shapefiles, per capita areas and census tract outlines)
2) the idf files generated from the Sustainable design lab at MIT (by Carlos Cerezo and Christoph Reinhart).

At the minute, all the data for 5 census tracts (which include the 1400 buildings) is included fro part 1, however the idf files are not yet included as they are quite large. 
I'll either add a download link at some point or you can email, but this wont be for a little while. 
Most likely it will be a zip file which contains the files to be added to the folder "Full_idf_files".

The readme will also improve once I get organised or if the paper is published.

