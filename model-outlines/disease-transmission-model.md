## Model Overview
 
### Purpose

A simple model of infectious disease transmission. Agents will move around a 2-dimensional surface and potentially spread an infectious disease to those nearby.

The model will manipulate the number of agents who move vs. stay in place (i.e. social distance) and observe the effect of social distancing on disease spread.
 
### Agents

A population of 200 agents will be generated. Agents will have a random position on a 2D surface.

Each agent will have an infection status (either susceptible, infected, or recovered); all but one agent will start the model as susceptible. One agent will start as infected.

All agents will also have a variable that tracks the number of days they have been infected; this will start at 0 for uninfected agents and 1 for infected agents.

Finally, all agents will possess a variable that reflects whether they are social distancing or not.

The proportion of agents that are social distancing will be set by a social distancing parameter.
 
### Life Cycle
 
1. Move
2. Infect
3. Recover

#### Move

Agents will move in a random direction. The distance they move on each day of the life cycle will be set by a movement speed parameter.

Agents that are social distancing will not move
 
#### Infect

Infected agents will potentially transmit the disease to susceptible agents nearby them. 

Only agents within a certain radius of an infected agent are at risk of transmission; 

This radius will be set as a parameter.

The probability of infecting each agent within this radius will also be set by a transmission probability parameter.

Only susceptible agents can be infected; infected and recovered agents cannot be re-infected
 
#### Recovery

The infection duration will increment by 1 each day an agent is infected. 

When the total duration exceeds an infection duration parameter, the agent will change status to recovered
 
### Analysis

The model will save the proportion of the population that is susceptible, infected, and recovered each day

These will be plotted as a function of time to observe both the rate of disease spread and the peak infected proportion as a function of the social distancing parameter.
