---
tags:
  - metaboflip
date: 2025-10-15
---
## goals and background
- I want to come up with a simulation that can realistically predict an individual's body temperature over time based on the conditions of its home range. 
- What I will be showing is very based on the [[Malishev et al. 2018]] paper on [[Methods in Ecology & Evolution]] with [[Michael Kearney]]. 
## simulation structure
1. An individual is dropped in a surface tile within its home range that is chosen based on the difference between the operative temperature of the tile $T_o$ and the $T_{pref}$ of all individuals. 
	- We can assume that $T_{pref}$ is ~ 32.5, which is the average body temperature we see an individual at during activity hours. 
2. Every simulation step (call them $t$) the simulation calculates the average difference between all surface tiles and $T_{pref}$.
3. If there are some surface tiles whereby the $T_o - T_{pref}$ difference is between $T_{act_{min}}$ and $T_{act_{max}}$ (which for our lizards can be calculated as the 95% confidence interval of the distribution of $T_b$ we have seen over time. $T_{act_{min}} = 27.5$ and $T_{act_{max}} = 35.5$) the lizard is on the **surface**. 
	1. All surface tiles are then ranked by $|T_o - T_{pref}|$ and their distance to the current tile. 
		- To expedite the calculation process, here, I can establish a cutoff and only include tiles between $27.5$ and $35.5$. 
		- For now the thermal quality of the tile and the distance are *weighed equally* when ranking.
	2. The ranking forms the basis of a probability distribution from which the next tile will be picked. 
		- We can define this probability of picking a tile using a Poisson distribution with $\lambda = 0.5$. This would make the best tile the most likely to be picked and the probability of picking other tiles would decline exponentially. 
	3. When a tile is picked that becomes the predicted $T_b$ at $t+1$. 
4. If there are no surface tiles that allow the animal to be within its activity range the animal is **underground**. The lizard has 2 possible depths available: 2.5 cm, 5 cm and the $T_o$ for this is derived from the surface $T_o$ using biophysical principles. 
	1. All underground tiles are filtered to only include those above the $CT_{min}$ of [[Sceloporus occidentalis]] at this latitude which we can set at about 4.5 C
	2. All underground tiles are ranked based on 3 criteria:
		1. Expected RMR based on each individual's RMR reaction norm (minimum preferred)
		2. Distance to the current tile (minimum preferred)
		3. Depth (closer to the surface preferred) 
	3. The same criteria is used to pick the tile in the next time interval and that is used to determine the position at $t + 1$. 
5. Re-run steps 1-4 for each hour of the day for the entire time when we have $T_o$ data. 
	- Important to determine what is an optimal time-step to run this. 
6. Re-run steps 1-5 at least 10 times per individual. 
## output of the simulation
- For each individual:
	- `simulation_run`: Boolean identifying the simulation number for that individual. 
	- `year`, `doy` & `mod`: Year, day of the year and minute of the day. 
	- `tb`: Predicted body temperature. 
	- `rmr`: Predicted mass-specific resting metabolic rate. 
	- `depth`: Predicted depth at which the individual is at (0 for surface, 2.5, 5).
	- `act`: 0 for sheltering, 1 for basking, 2 for activity. 0 will always be assigned if underground, 1 will be assigned is the animal is on the surface and its predicted $T_b$ is below 1 C of $T_{pref}$ and 2 if the animal is within 1 C of $T_{pref}$ and thus active. 
## potential validation against real world data
- We can check the average distance of each actual individual observation to the locations the simulation has predicted. 
- We can also compare the body temperature we measured in the field to the average predicted body temperature across multiple simulations. 