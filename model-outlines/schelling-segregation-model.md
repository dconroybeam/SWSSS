## Model Overview

### Purpose

Determine whether segregation can be explained by individual motivations to avoid being a local minority. Agents will move around a two-dimensional space depending on whether they are a racial minority within their local neighborhood.
 
### Agents

A population of agents will be generated; each agent will have a race (black or white) and a position in a 2-dimensional space.
 
### Life Cycle
 
1. Assess
2. Move
 
#### Assess

Each agent will first calculate how far they are from each other agent in the 2D space. The agent will then identify all agents who reside within a set radius around them. These agents constitute the focal agent's neighborhood.

The focal agent will then determine the race of all agents in their neighborhood. Finally, the agent will determine whether they are in the minority race in their neighborhood.

#### Move

In this stage of the life cycle, the agent makes one decision: if the agent is not in the minority then they will stay where they are. If the agent is in the minority, they will move to a new random location.
 
### Analysis

The model will plot the position of agents before and after the movement phases
