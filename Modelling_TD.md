# Modelling the data

### Skill metric

For the Skill Index, when determining the skill level for each player, a weighted sum approach was used that employed the normalised statistics provided. The coefficients varied for each skill's aspect (shooting, passing, defending, goalkeeping) and position. An additional weighted sum for a total skill score was then calculated to aggregate all data. The coefficients were calculated utilising actuarial judgement, that considered the value of the metric through research and exploratory analysis of the skills stronger teams possessed in the tournaments, e.g. highest weightings were applied to skill success rates; weaker weightings to less desirable features. Some weightings were also applied to metrics that did not necessarily indicate skill but expressed a desirable level of experience as this would prevent selection of players that might have excellent success rates but very low attempts, e.g. 100% tackle success rate but only 2 total tackles attempted. This modelling was used for each skill area with weightings assigned based on the relevance of the statistic for the player, e.g. it is more critical that a forward is making tackles in the attacking third rather than the defending third. Further, many variables were perfectly correlated with each other such as the total tackle count and counts of tackles within each third. Their coefficients were set to account for multi-collinearity. 
This approach was chosen as there were no distinct response variables that could be used to model player skill levels other than a team’s tournament performance. Once these scores were created for each skill aspect, they were then added together in an additional weighted sum based on the importance of that aspect for the position such as how forwards need excellent shooting unlike defenders. Players were then ranked by total skill component and its simplicity is valuable due to its allowance for future adjustments as new skills may become more relevant for other matches.

The process for how the statistics were normalised and how the skill index was produced can be found [here](Modelling_Skill_Metric.R).

![](Tackle_Nation_Level_Graph.png)

The code begins by reading in all the data, normalising each relevant statistic, producing the individual skill area scores by position and then finally creating the total skill metric score. [DO WE WANT AN EXPLANATION OF THE CODE???]

## Should this portion below get moved to more an exploratory data analysis section or just the start of the modelling section

Visual analysis was first utilised to explore the data and brainstorm potential methods for modelling the data. Initially visual scatterplots were used to determine the importance of variables by observing each player’s normalised score for a statistic and their team’s position in the global tournaments. This analysis showed no prominent patterns across most statistics and showed some biased patterns across defensive statistics such as number of tackles. A defender should be capable of making tackles but weaker teams are generally more likely to be on the defensive and will naturally make more tackles, making it seem like a player is worse for having made more tackles. 


## Limitations Report + Everything
There were several data limitations, including missing data for some simple statistics, e.g. basic physical statistics. While skill is important, physical potential can guide further decisions as certain physical traits cannot be improved (e.g. height) and thus, players can be chosen with desirable traits, e.g. taller people for forwards to receive crosses. Simplicity of the data is considered a limitation, as seasonal performance rather than game by game performance does not show the variance of a player’s ability and contribution to win/loss ratios. Moreover, only two years of football data available, making it difficult to analyse optimal choice of players and number of players in each position for tournament success.

Economic data availability from more years would permit more complex models to better understand which metrics influence which variables and forecast more accurately, e.g. increased data on exchange rate, revenue, expenses (beyond 2016-2020) as well as GDP and population (beyond 2011-2020). 



## Future Outlook - Probably can just report but then tack on 1-2 sentences for further detail. 2-3 sentences that relate to the 'self-contained' portion of the marking criteria -- Potentially making direct references to ease of updating the models? Look into how other finish their github pages in general.

Through utilisation of these recommendations, Rarita should see large improvements in their national football performance, subsequently boosting their economy. This strategy was designed flexibly so that it can be adapted to any new problems or focus areas for team selection that arise. Furthermore, the additional remnants of the budget can be allocated to areas such as further training to boost probabilities of winning or new exposure opportunities, compounding the positive effect of popularity on the economy. Thus, Rarita now has a comprehensive plan to establish a world-class football team and host a future World Cup which should reap substantial benefits to its economy.
