---
tags:
  - unc-riddell
  - smith-noaa
  - research
date: 2025-05-29
people: "[[Eric Riddell]]"
relates to:
  - "[[idea dump about Marie-Curie proposal]]"
  - "[[first meeting unc-riddell]]"
---
for a fully finalized version with feedback, go to: https://docs.google.com/document/d/16o-Xfst5BTa_4MQPbuXHTMXBUu-TYN97vlDuEq1kAak/edit?tab=t.0
# general framework
- Thermal reaction norms and thermal tolerance vary across life stages in all ectothermic organisms. 
- Taking lizards as an example, TPCs of embryos and adults differ in their $CT_{min}$ (always warmer in embryos), $T_{opt}$ and $CT_{max}$ (always cooler in embryos). 
- Empirical evidence shows that adults alter behavioral thermoregulation during gestation to favor embryonic development. 
	- There is evidence that this happens towards the embryo's $T_{opt}$ ([[Pettersen et al. 2023]]) but less so with respect to the $CT$s. 
- This forces mothers to experience a suboptimal $T_b$ distribution with respect to their physiology, which should have a towards  survival.  
	- Gestation also might affect the mother's survival via other mechanisms like increased energetic expenditure or higher risk of predation.  
- From the embryo's perspective, increased gestation will always improve fitness, due to the more favorable conditions the mother provides compared to those it would experience if laid in a nest. 
	- Note that "more favorable conditions" is not limited to warming embryos (cold-climate-hypothesis) but also to cooling them (in particularly hot environments), minimizing thermal fluctuations, controlling humidity levels and minimizing predation etc.
- As such, a **thermal reproductive conflict** arises between mother and embryo which is exacerbated by a suboptimal environment for embryo development. Lengthened gestation leads to greater offspring fitness (e.g., greater hatching success of condition at birth), but this comes at the expense of the mother's survival and future reproductive chances. 
	- See my viviparity model paper to see how this balance is resolved into an optimal gestation length strategy. 
- However, extending gestation is likely extremely costly or unfeasible due to phylogenetic or physical constraints. 
- As such a mother will probably exhaust every other possibility to improve the thermal regime under which embryos develop before resorting to it. In my view, a mother has several behavioral / plastic mechanisms to achieve this: 
	1. Change the habitat it occupies (if possible). 
	2. Change its reproductive phenology within a habitat (e.g., reproduce early). 
	3. Change its thermoregulatory behavior (e.g., bask more or less to the extent to which it can). 
	4. Change oviposition sites (e.g., alter the depth, shade coverage or substrate in which eggs are laid). 
- Alternatively, a female can reduce the cost of carrying eggs through evolutionary (perhaps even plastic) mechanisms like: 
	1. Increase in size so eggs represent a smaller percentage of body mass. 
	2. Carry fewer eggs for the same reasons. 
- To mediate the thermal reproductive conflict, a lizard might assume one or other set of *reproductive strategies* that can be behavioral, plastic or evolutionary. However, the application of these strategies will be dependent on the characteristics of the environment it inhabits. 
- This leads me to 4 major unanswered questions to ask:
	1. **To what extend do lizards alter reproductive strategies due to the environments they inhabit?**
		- e.g., do lizards living in suboptimal environments alter their phenology of reproduction? do they alter thermoregulatory behavior? do they alter nesting strategies? have they evolved alternative life histories?  
	2. **What is the effect of a given reproductive strategy?**
		- e.g., by how much does breeding earlier improve the conditions an embryo experiences in the soil? by how much modifying nesting sites improves embryo development? how much less energy does a female spend by having producing one fewer offspring? 
	3. **Have there been changes in reproductive strategies as a result of recent climate change?**
		- e.g., by how much have lizards changed reproductive phenology over the last century? what about nesting strategies? what about life-history traits? what has been the effect of these changes?
	4. **Can we forecast how reproductive strategies might shift as a result of future climate change? 
		- e.g., will lizards continue to alter reproductive strategies or these strategies might not be enough to withstand future changes? Can we use this to obtain more comprehensive population forecasts? 
- Everything above can be to some extent summarized in the diagram below:
![[smith-noaa-proposal-diagram.svg]]
# project 1: smith / NOAA fellowship
## fellowships to apply to 
1. [Smith Conservation Research Fellowship](https://www.smithfellows.org/)
	- Sponsored by the Society for Conservation Biology
	- Proposal would need to be focused on a conservation aspect. 
	- Comes with $40K in research and travel funds. 
2. [NOAA Climate & Global Change (C&GC) Postdoctoral Program](https://cpaess.ucar.edu/cgc)
	- Sponsored by NOAA and the University Corporation for Atmospheric Research. 
	- Proposal would need to highlight the global change aspect of the project and the use of macroecological data. 
	- Potentially subjected to budget cuts and overall cancellation. 
	- $8K / year in research and travel funds. 
- Both fellowships allow for co-sponsorship, based on the ideas I have, I think that a good co-sponsor would be someone who is either:
	1. An expert in statistical modelling of phenological changes over time: Some candidates would be Dr. [[Alexa Fredston]] or Dr. [[Casey Youngflesh]]. 
## questions
1. **Have there been changes in lizard reproductive strategies along macroecological gradients over the past century?** 
2. **Why have lizards altered (or not) their reproductive strategies? 
	- What has been the consequence of altering a reproductive strategy? e.g., how much soil temperatures have changed between now and 50 years ago during the months when lizards reproduce? Are lizards capable of buffering the impact of climate change by altering phenology? 
3. **Can we forecast how lizards might respond to future changes in their environments along macroecological gradients to infer population viability?**
## tentative research plan
1. **Obtain data of lizard reproductive strategies in the past**. This can be achieved via two data sources:
	1. **Past demographic studies**: 
		- Studies quantifying the demographics or reproductive cycles of lizard populations. 
		- There are *hundreds* of these studies and they extend as far back as the 1940s all the way to today although there is a heavy bias (most studies in US). 
		- Most studies report similar information I could record, for example: 
			1. Basic taxonomic, temporal and spatial information. 
			2. Phenology of reproduction (e.g., when did copulations happen, what percentage of females where gravid, what percentage of the captured individuals were juveniles etc.)
			3. Life-history traits (e.g., female mass or SVL, egg number, egg diameter etc.)
			4. Behavior (e.g., activity patterns, daily abundance etc.)
	2. **Museum specimens**: 
		- Museums across the US and other countries keep specimens collected since their establishment. From each specimen I could obtain: 
			1. Basic taxonomic, temporal (date collected) and spatial information (location of collection). 
			2. Phenology of reproduction by assessing presence or absence of eggs on females using an ultrasound or X-ray scanning. 
			3. Life-history traits (e.g., female SVL, egg number and diameter through ultrasound or X-ray scanning)
		- Like in the case of past demographic studies, the sample could be potentially biased towards the US. 
2. **Obtain data of lizard reproductive strategies in the present**. This can be achieved via two data sources:
	1. **iNaturalist**:
		- Through iNaturalist I can obtain the following data:
			1. Basic taxonomic, spatial, temporal (even hour of the day) data. 
			2. Phenology through number of observations / day. 
			3. Demographics via tags on observations (e.g., sex, life-stage).
		- To model this data I would need to account for detection probability and make spatially and temporally explicit models, hence the need for an expert. 
	2. **Re-surveying populations where demographic studies were conducted**: 
		- If located in the western US, I could access a decent number of populations and do monthly surveys following the same methodology as past studies but using non-invasive techniques like ultrasounding to assess reproductive status. 
3. **Obtain past and present data to run microclimate models**:
	- Some data types that could be of interest:
		1. Temperature, precipitation, wind etc. at appropriate scales. 
		2. Terrain slope, roughness, elevation etc. 
		3. Soil depth and properties. 
		4. Vegetation cover - Could be used to assess shade cover. 
4. **Use microclimate and dynamic energy budget models to re-construct the environments experienced by lizards**
	-  Using microclimate models I could estimate:
		- Changes in nesting conditions. (e.g., a consequence of changes in temperature + vegetation cover + breeding phenology). 
		- Use climate change predictions to estimate how nesting conditions will further change in the future 
	- Using dynamic energy budgets + results of microclimate models I could estimate:
		- Changes in the energetic costs of reproduction (e.g., metabolic expenditure, availability of basking sites etc.)
	- All the above would be estimated in as many species and populations as possible comparing past and present data. 
	- The final goal would be to build physiological maps that could be translated into "reproductive suitability maps". Ultimately I envision a spatially and temporally explicit species-specific prediction of population viability. 
## next steps 
1. Draft a general proposal outline compatible with both Smith and NOAA Fellowships
2. Contact a potential co-sponsor. 
	- I've thought about Dr. Casey Youngflesh and Dr. Alexa Fredston. 
3. Draft outline for Smith and NOAA proposals independently ~ Late June / Early July
4. Complete Smith Proposal ~ Late August, early September. 
5. Submit Smith Proposal by September 30th 2025. 
6. Complete NOAA proposal ~ Late October 2025
7. Submit NOAA proposal ~ January 10th 2026. 
# project 2: Marie Skłodowska-Curie Actions
## fellowship details
- Sponsored by the EU
- Requires co-sponsorship, best option [[Miguel A. Carretero]]. 
- Details: “They fund the mobility of researchers outside Europe. The fellowship lasts between 2 to 3 years, of which the first 1 to 2 years will be spent in a non-associated Third Country, followed by a mandatory return phase of 1 year to an organisation based in an EU Member State or Horizon Europe Associated Country. Only nationals or long-term residents of the EU Member States or Horizon Europe Associated Countries can apply.”
	- I hope I can flip the script and collect the data first and then go to the US. 
## background
- Tenerife lizard (*Gallotia galloti*), endemic to the island of [[Tenerife]] in the Canary Islands, territory of Spain. 
- Tenerife is an oceanic island with a volcano on the middle of it (Mount Teide, 3715 m tall) and an mountain chain cutting the island in half on a NE-SW direction
- The prevalence of trade winds blowing N-S generates drastically different environments across both slopes of the volcano and mountain chain. N slope is cool and wet with and relatively forested. S slope is hot and dry, and dominated by xeric vegetation.  
- Lizards are locally abundant (based on iNaturalist records) and distributed all across the island, in both slopes and at elevations ranging from sea level to over 3000 m.
	- Some studies suggest that the lizards of the northern and southern slopes are subspecies but I do not believe in subspecies anyway. 
- Tenerife offers the perfect environment to study if and how lizard reproductive strategies are influenced by climates. 
![](https://lh7-rt.googleusercontent.com/slidesz/AGV_vUcv0YWWR2M9AAYHwrHt2-eViet_9d5idhCKNLcIUx4OthzmOceX6oeo6qGkHhKwjo8N_iw1zHLF0qXl9qlX_GDVf_-Y5DzDrAaL6ffweaUqFGL4YQXgUdMR2-qqUgvwSjzo80b6pQ=s2048?key=SOHw9kQFKQnO0K4rTLShvg)The trade winds blowing in the N-S direction acting on Tenerife generate vastly different habitats. 
![](https://lh7-rt.googleusercontent.com/slidesz/AGV_vUe_YrVxY1lJrGSlEYtGn6giCAO_k7lwG93_IHkI958INUF01RMgVSsYWyCtObsnocBhUc-svsrtEF2p768pAfm4wGQWiiN2NFcNmIeQW9nP9_vJchbAwr7JClVpnnaq-YW1chfI1A=s2048?key=SOHw9kQFKQnO0K4rTLShvg) iNaturalist observations of [[Gallotia galloti]] indicating that the lizard is present all over the island regardless of habitat type. 
## questions 
1. **Are there differences in reproductive strategies along environmental gradients?**
2. **Why are or aren't' there differences in reproductive strategies?**
3. **Can we forecast how changing environments might influence reproductive strategies and with that forecast population viability?**
## tentative research plan.
1. **Conduct fieldwork to obtain data on** (from highest to lowest priority):
	1. **Life-history traits**: Differences in body size, offspring number, egg number and size etc. Much of it using a a hand held ultrasound
	2. **Phenology of reproduction**: Conduct surveys to get abundance estimates, assess population size distribution and, using an ultrasound, assess reproductive status. 
	3. **Thermoregulatory behavior**: Body temperature x reproductive status, microhabitat use, activity patterns etc. 
	4. **Environmental data**: Soil depth, terrain roughness etc. if that data is not available publicly or, if it is, complement it. 
	 Ideally, I would conduct a replicated effort across 5-10 populations located along environmental gradients over an entire year (or more) cycle. 
2. **Use microclimate and dynamic energy budgets to model how different environments impact lizards and embryos**. And with that answer *why* do reproductive strategies differ, if they differ at all. 
	- Basically the same approach (nesting temperatures, energetic costs of reproduction etc.) as discussed for the first project. 
	- An advantage of working with this species in particular is that there is already extremely high quality data on $T_{pref}$, EWL, Coloration (Reflectance), Body mass, Oxygen consumption etc. 
3. **Forecast how changes in climate might influence reproductive strategies across different habitats**
	- Is it possible that climate change might lead to environments too hot for eggs? Will this influence gestation and thus reproductive costs for females? Will this lead to population decline? 
	- Multiple species of *Gallotia* lizards in the Canary islands, some of them critically endangered.