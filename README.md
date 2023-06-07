# robotics_final
Final deliverables for Robotics 2023

The delivered files consist on the following:

main.ttt
--------
This is the main CoppeliaSim scene. The scene contains a dummy object with an associated pyhon script that sets up the scene and loads our models, as well as managing the simulation (food retrieval, removing predated agents, ...).

In order for the simulation to run, CoppeliaSim is required (we have used CoppeliaSim Edu, version 4.4.0) with the Python interpreter set*.


*This last step is made by changing the "defaultPython" parameter in the file in "./CoppeliaRobotics/CoppeliaSimEdu/system/usrset.txt" with the path to the absolute path of your 'python.exe' file, as well as pip installing the required python modules.
More information on this thread: https://forum.coppeliarobotics.com/viewtopic.php?t=9614




models folder
-------------
This folder contains the models created for the simulation:

·swarm_agent.ttm
This is the main swarm agent ant model. It includes the behaviour script and the 360º camera with its own sensing stript.

·predator.ttm
This is the main predator ant model. It includes its behaviour script, that differs from that of the swarm agents, and the 360º camera with its the sensing stript, which is a direct copy of that created for the swarm agents.

·food.ttm
This is simply a placeholder that is placed where the food source is in order to be identifiable by the agents via computer vision.
