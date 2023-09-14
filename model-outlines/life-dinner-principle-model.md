## Model Overview
 
### Purpose

Observe the "life-dinner principle": in coevolutionary arms races, prey animals have the advantage in that they are fighting for their lives whereas predators are just fighting for dinner.

Agents representing rabbits and foxes will have random encounters with one another. Whether the rabbit escapes--and whether the fox eats--will depend on their relative speed.

Rabbits will reproduce only if they survive; foxes will reproduce only if they get enough to eat.
 
### Agents

Agents will represent either foxes or rabbits. Each agent will also have a speed variable randomly assigned to them from a normal distribution. Rabbit agents will possess a variable that determines whether they have been eaten; foxes possess a variable that tracks the number of rabbits they have eaten.
 
### Life Cycle
 
1. Encounter
2. Eat/escape
3. Reproduce/Die
 
#### Encounter

During this life stage, each fox will encounter one rabbit at random. 
 
#### Eat/Escape

The model will next determine whether the fox eats its encountered rabbit or whether the rabbit escapes. The model will roll dice for each agent with the maximum value equal to the agent's speed value.
 
If the rabbit's dice roll is higher, the rabbit escapes; otherwise the fox eats the rabbit. 

The total number of encounters a fox experiences will be set by a parameter.
 
#### Reproduce/Die

After encounters are resolved, the agents will reproduce. Rabbits will reproduce only if they survived. Foxes will reproduce in proportion to the number of rabbits they ate.

Offspring will inherit their speed variable from their parents.

### Analysis

The model will compute the average speed of foxes and rabbits within each model run.
