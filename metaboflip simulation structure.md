---
tags: 
date: 2025-10-15
---
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
	1. All underground tiles are filtered to only include those above the $CT_{min}$ of [[Sceloporus occidentalis]] at this latitude which we can set at about 5
	2. All underground tiles are ranked based on 3 criteria:
		1. Expected RMR based on each individual's RMR reaction norm. 
		2. 