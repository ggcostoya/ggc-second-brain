---
tags:
  - metaboflip
date: 2025-10-14
people:
  - "[[Mike Logan]]"
type:
  - meeting
---
## meeting prep
- calculating home ranges 
- penalizing behavioral thermoregulation over space. 
- reliability of crevice OTMs and using other methods to quantify underground temperatures. 
- what temperatures should the lizards assume at night. 
- food availability
### thermoregulatory behavior
- The issue is that a given individual has equal chance of arriving at a habitat patch at the optimal temperature regardless of how car the patch is to its current position. 
- An alternative would be to run a simulation where an individual is placed in a starting point and it can only move a certain area from the spot where it is at a given time step - this would be essentially an adaptation to the [[Malishev et al. 2018]] paper on [[Methods in Ecology & Evolution]] with [[Michael Kearney]]
- If doing the above, the time frame of the step is critical. I've been running hourly models for now and, based on what we know about the lizards they can (not necessarily will) move the entire length of their home range within a one hour period. 
- If we assume that, then assuming that the lizard can find the optimal patch throughout its entire habitat is relatively reasonable. 
- An alternative thing we can do to introduce stochasticity is to filter all possible tiles within a range of values close to where the lizards wants to be at and weigh them by distance to determine which one will the lizard choose. 
- But this runs into the problem of surface vs underground temperatures: When does the animal make the decision to go aboveground vs go underground?
- Movement is constrained underground substantially so we can assume that the animal cannot move without hitting the surface. 
- We need to establish some rule of thumb by which the individual either stays aboveground or goes underground based. 
- Is the amount of distance a lizard can move determined by its body temperature?
- IF we do any kind of simulation, we would need to run it multiple times per individual. 
### what temperatures should lizards assume at night?
- If it can be reached 