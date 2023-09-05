## Model Overview 
 
### Purpose

The purpose of this model is to explore the emergence of fads as a function of varying levels of conformity and anticonformity.

Agents will choose between three options (grow a beard, grow a mustache, or be clean-shaven) based on one of two conformity strategies. Some agents will be "conformists": these agents will adopt facial hair styles in proportion to how popular they are in their social group. Other agents will be "hipsters": these agents will adopt facial hair styles in proportion to how unpopular they are in their social group.
 
### Agents

A population of agents will be generated. Each agent will have a strategy: hipster or conformist. The population size, proportion of hipsters, probability of changing hairstyle, and social group size will be determined by manipulable parameters.

Agents will be assigned to random social groups; social groups will be non-overlapping such that not all agents within a particular agent's social group will mutually know one another.
 
### Life Cycle
 
1. Assess
2. Switch
 
#### Assess

Each agent will first assess the facial hair of all other agents in their social group. The agent will then determine the proportion of agents who have beards, mustaches, and are clean shaven.
 
#### Switch

After all agents have assessed the population, each agent will switch their facial hair based on their conformity strategy.  

The probability of agents changing their facial hair each month will depend on a manipulable parameter.  

"Conformists" will choose a random facial hair style with probability directly proportional to the proportion of agents in their social group with that facial hair style.  

"Hipsters" will choose a random facial hair style with probability inversely proportional to the proportion of agents in their social group with that facial hair style.  

In this way, conformists will tend toward wearing whatever is most popular whereas hipsters will tend toward wearing whatever is least popular
 
### Analysis

The model will plot the proportion of agents wearing each facial hair type as a function of time.
