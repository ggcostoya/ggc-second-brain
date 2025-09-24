---
tags:
  - how-suboptimal
date: 2025-05-21
---
- The shapes of [[TPC]]s must evolve to maximize fitness under the thermal conditions an organism experiences. 
	- Within the potential set of constraints that the [[TPC]] shape might have
- As a result, hypothetically, we could deduce the temperature distribution (or set of) that would lead to a [[TPC]] maximizing its fitness but how can we do that?
- The impact of thermal variability - [[Jensen's inequality]] on [[TPC]]s - in a variable environment $T_{opt} < \hat{T}$  based on previous research but what about other aspects of a temperature distribution like its skewness or bimodality? Both aspects that have been largely overlooked.
- Why care about skewness? - Behaviorally thermoregulating animals experience inherently skewed distributions during day-time hours - Very left skewed curves. 
- Why bimodality? - Behaviorally thermoregulating animals or organisms experiencing two clear.
- Here:
	- We explore how [[TPC]] fitness is influenced by both skewness and bimodality in addition to mean and thermal variability. 
	- We use real [[TPC]]s to explore what is the temperature distribution under which they should have evolved to maximize fitness. 
	- We compare the latter temperature distribution to temperature distributions drawn via different methods (pulling macroclimatic variables, ecophysiological modeling etc.) with the goal of answering what is the best possible way to represent the temp. distribution that should have led to the shapes we observe. 
## methods
### analysis of empirical data
- We obtain [[TPC]] data of terrestrial ectotherms from [[Buckley et al. 2022]]. 
- We simulated environmental temperature distribution for each [[TPC]] using the software [[NicheMapR]]
	- We can grab the `metout`, `shadmet`, `shadsoil` etc. objects to obtain these temperatures. 
- We also used [[NicheMapR]] to run the `ectotherm` model on each using the best parameters we could find
	- We can start with lizards here and go from there to expand to both insects and plants. 
- From each temperature data we obtained we obtained a `density` estimate of each temperature between -50 C and 100 C at intervals of 0.1. 
	- We got these density estimates for both environmental temperatures and temperatures estimated via the ectotherm model. 
- We then explored, among the range of possible [[TPC]] shapes which shape would maximize fitness under a given temperature distribution. 
- We compared that shape to the actual shape of the organism by its constituent parameters $CT_{min}$, $T_{opt}$ and $CT_{max}$. 
- We assessed which kind of temperature distribution led to the smallest difference in the [[TPC]] shape that would maximize fitness under that temperature distribution and the actual [[TPC]].
- We explored how these patterns differed across latitudes, longitudes, elevations and organismal behaviors. 