## Model Overview
 
### Purpose

Determine whether assortative mating can emerge from individual mating motivations. Agents will select one another as mates based on a physical attractiveness variable.

Each agent will pursue mates probabilistically and in proportion to mates' physical attractiveness. The model will then calculate the extent to which agents mate assortatively for attractiveness.

For comparison, the model will also assess assortative mating for randomly formed pairs.

This model is based loosely on Kalick and Hamilton (1986).
 
### Agents

Each agent will have two randomly assigned features: sex and physical attractiveness. Half of all agents will be male and half will be female.

Agent physical attractiveness values will be drawn from random uniform distributions constrained between 0 and 10.

Agents will also possess a maximum number of dates they will tolerate going on before settling for any mate.

Agent selectivity will gradually decline as they approach their maximum number of dates.

### Life Cycle

1. Date
2. Offer
3. Pair
 
#### Date

At the start of the life cycle, a random agent will be paired with a random opposite-sex partner. Dating agents' number of dates will be incremented by one.
 
#### Offer

Next, each dating agent will decide whether to make a long-term commitment offer to their dating partner. The probability of making an offer will be proportional to their date's attractiveness, adjusted by the number of dates the agent has gone on.

If an agent has reached their maximum number of dates, they will make an offer to their next date regardless of attractiveness.

#### Pair

Finally, dating agents will pair if both agents mutually make long-term commitment offers to one another.
 
The life cycle will repeat until all agents are paired
 
### Analysis

The model will compute the correlation between male and female attractiveness within couples for each model run. Correlations across model runs will be plotted with a histogram.

The model will also randomly scramble agent couples and compute the attractiveness correlation for random pairs within model run. 

These random choice correlations will be plotted alongside the attractiveness-driven results for comparison.
