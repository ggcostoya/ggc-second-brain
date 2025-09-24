---
tags:
  - metaboflip
  - flip
date: 2025-08-26
people:
  - Mike Logan
  - Akhila Gopal
type:
  - meeting
---
- To justify the fact that we are going to drop some trials we will say that we did not leave enough time to equilibrate between major temperature swings (e.g., between 40 and 20, when most errors occur).
- One of the cut-off things we are going to do (in addition to dropping all RMR < 0) is to cut all rates where the rate at the greater temperature is lower. 
- I will perform a cross-validation of individuals with 4 temps, remove one out etc. to verify that predicting with 3 temperatures is a sound approach. 
- If the results of the above are valid, I'll calculate the wrong rates for individuals and check if they fall close to the mean. 
- I also need to check with Akhila about preparing all the OTM data - I just need to run `rnp_otms_data` with all the 2023 OTMS data - I must have the script I used to calculate rates somewhere. 
- Big debate about this result: 
- ![[Pasted image 20250826115437.png | 500 x 500]]
- I think, there is an evolutionary constraint going on here where slope and intercept are negatively correlated, the question is why.
- Might be worth revisiting the [[Plasman et al. 2020]] paper looking at [[Sceloporus grammicus]] metabolic rates at different elevations. 
- My idea here is that individuals that experience lower body temperatures on average have higher intercepts because that's the only way you can achieve the same optimal activity in a cooler environment assuming that slope and intercept are constrained. 
- Need to have a better answer for this. 