---
tags:
  - flip
  - metaboflip
date: 2025-07-04
people:
  - Mike Logan
  - Akhila Gopal
  - Noa Ratia
type:
  - meeting
---
## defining individual home ranges
- slide 3:
	- One of the core principles of our project is understanding how thermal environments influence specific individuals. 
	- As such, we need to be able to determine what is the space occupied by that individual in order to understand the environment within it. We do that by determining an individual's home range.
	- Based on the research I've done, the two methods that could work for our purposes are minimum convex polygons (MCP) or Kernel Density estimates (KDE)
- slide 4:
	- Briefly, MCPs represent the convex hull that encompasses all of an individual's observations while KDE is a probabilistic function that determines the probability of a point space being part of an individuals home range based on where it has been seen. 
	- Both approaches are doable and work more or less with our data but they both have pros and cons as highlighted in the list above. 
	- The plot to the left of the screen shows the home-ranges of individuals within the old area of the LE site for which we have at least 5 captures using MCPs and KDEs. MCPs and KDE areas are color coded by individual ID. 
	- Note that the KDE is dependent on a core % value. This core % value describes all areas where there is a > X chance of that area being part of an individual home range. For this plot I chose 50% as otherwise the estimated home ranges would be massive. See why on the next slide. 
- slide 5: 
	- To illustrate some of the issues with MCPs and KDEs here I show 3 individual home ranges of 3 famous lizards. The polygon-like shapes are the MCPs whereas the circle-like shapes are the KDE estimates. The points show the positions in which we have recorded that individual. 
	- For Scoobs, the KDE method works well and yields a result similar to the MCP as most observations are more or less uniformly distributed across a small area. 
	- For L048 the KDE method is terrible as it returns a circle, likely caused by the 2 observations that are far far away from the rest. I double checked to make sure that the two observations were correct and indeed they were. 
	- For L089, it is basically the same problem as with L048. The KDE method fails to capture what I call "extremes" or  positional "outliers". 
## meeting notes
- MCP vs KDE: The guiding principle should be if an area is meaningful for an individual from an evolutionary and ecological perspective. 
- Not every animal needs to be included if you are not confident that the individual was staying there
- Run the analysis using both MCP and KDE. 
- Eco-Evo perspective KDE makes more sense. 
- 50% KDE sounds like a good approach - 75% works too. 
- Theory underlying KDE - what is meaningful. 
- 3 datasets - 50%, 75% and MCP. 
- Number of captures is important - might matter. 50% of low number of captures, 75% if more captures. 
- How many captures. 
- In terms of thermal environments we have to show that individuals experience vastly different temperatures within the same habitat. 
- Tpref values must be reliable. 
- Can Tpref be cleaned up. 
- When they first emerge they have Tpref. 
- Rely on HE value for Tpref. 
- Averaged Tpref value for all. 
- Do not include lizards that are below a certain value - throw individuals out. 
- Penalize movement between spots - cost of reaching that temperature as a function of the percentage of spots in the site that are at an optimal temperature. 
- Sears paper - Random forest approach to simulate how an animal might move through these patches. Spatially explicitly ask how likely. 
- Parameterize costs of movement - 
- We can assume that costs of movement are not penalized. 
- Dynamic body temperature prediction - good enough. 
- Grain size - 
- Simulation approach to test stuff? dynamic reaching tb. 
- Separate estimate of thermal grain size - 
- Equation based metric of thermal quality - 
- Average patch size of areas at the same temperature. 
- To quantify crevices - Go to the site and check them out. 
- assume that this is the average crevice temperature. 