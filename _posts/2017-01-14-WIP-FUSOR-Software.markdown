---
layout: post
title:  "WIP: FUSOR software - Update 1"
date:   2017-01-14 00:00:00 +0100
categories: jekyll update
---

Introduction: The TU/e fusor is a IEC fusion decise. This means that fusion of deutrium is done be electro static confinement. To do this a metal grid (tungsten) is suspended in a vacuum where an high voltage set on. A part of the remaining gas is a bit ionised and therefore accelereated towards the grid. Near the grid the ions can collide with other ions or with neutral gas particles. In case the collision energy is high enough fusion can occure. 

Goal of the software: Operation of the fusor is slowsly becomming more complex and difficule to opperate pure by hand. Many diagnosics needs monitoring, serveral controling tasks carried out and logbook to be filled in. This last tasks has become an importand tasks as the radiation produced by the fusor can be harmfull and carefull log data gives an overview of the dosis produced. However clear logging of all this data is diffucult and prone to errors. 

To reduce the errors in the logs and free the operators from these time consuming log tasks so they can fusor on the 'real' science, an program is developed. This program is should carry out some basic tasks such as logging of pressure, voltage, currents and neutron production. Further allow for simple controling the pressure. The advanced tasks could be the logging of the video feed and controlling the PSU self by a programmed shot scheme. 

Design choises: The software is completly written in Matlab code. This because serveral reasons. Coding in texts is (in my opinion) better that graphic programming like LabView. The second reason is that Matlab is more known to the studens of the TU/e that will work on the fusor and therefore the continouty of develepment is better garenteed. The drawback of this choise is that Matlab is a bit less suited for controlling perposes than LabView. 

Current status: Logging and controlling the pressure is the first thing that was completed. This is working fine and without issues. 

The logging of the voltage, current and NPR got a major overhaul in the last big update. More about this can be found in the svn logs, or I'll perhaps write a more detailed log about in the future. The short version is that it now works in both 'continous' and 'shot' mode. 

Intergrating the video feed in to the data logging descriped above is still in the design phase. Some simple test have been carried out to enable comminication between the 2 computers which works fine. Some discussion is needed about the layout of the second interface and its functionallity. Using Matlab to view the webcam is possible but it's unknown how rubust this is when the webcam fails through emissions of the fusor. 





