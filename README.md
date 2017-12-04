# Create a species capture history from eMammal data 

---

#### This repository is to be used for creating a species capture history (aka "detection history") from eMammal data.  

---

[eMammal](www.emammal.si.edu) is a data management system and archive for camera trap research projects, and is where the [North Carolina Candid Critters](http://www.nccandidcritters.org/) project stores their data.  

#### For information on how to access eMammal data, see this video: 
<a href="http://www.youtube.com/watch?feature=player_embedded&v=c2HsqLnm51w
" target="_blank"><img src="http://img.youtube.com/vi/c2HsqLnm51w/0.jpg" 
alt="Using eMammal website" width="240" height="180" border="10" /></a>

### Repository Contents:

1. An R script ```Create_Capture_History.R``` for creating the capture history 
2. Example datasets. The datasets are outputed directly from eMammal's [browse data](http://emammal.si.edu/analysis/data-download) tab.  
2a. ```example_data.csv``` is a selection of North Carolina Candid Critters data.  
2b. ```example_data2.csv``` is all North Carolina Candid Critter's data as of 11-19-2017.   
3. A 'Capture Histories' folder where the script output will be stored. This folder may have existing output files in it. The files were likely created when demoing this repository. You may discard them as you see fit.
4. A .csv file ```Eastern_NC_counties-LiDARcutoff.csv``` listing the counties that are currently (Dec 2017) covered by lidar data. This file will be called if you only want a detection history for Eastern North Carolina. 

### Repository workflow:  

1. Download data from eMammal and store with this repository. If the .csv file fethed from eMammal is altered in anyway, it may not work with script. 
2. Change line 17 of ```Create_Capture_History.R``` to reflect the name of your .csv file.
3. Source ```Create_Capture_history.R```
4. Retrieve capture history from 'Capture Histories' folder.




