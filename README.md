# HiveSimulation
Model a stochastic process using random agents. This project is inspired by the behavior of termites that gather wood chips into piles.

When running the simulation, it can be seen that the starting point has a distribution of wood throughout the hive without any particular shape or formation. As the termites fly and move woods within the hive, clusters of woods begin to form. These clusters have curved shapes. 

At the end of the simulation you have these formations between the woods as the termites move them and place them near other woods. In doing so, the spaces near clusters of chips tend to fill in, forming inner clusters of chips with no free spaces around them in the center of the clusters.

The number of piles decreases with time given the conditions of the simulation since termites can randomly remove any wood that is next to an empty hive space and this same wood is placed in an empty space that has woods around it. For this reason, chips will clump and compact over time as any chip can be removed but must necessarily be placed next to another chip. As chips are placed close to each other, larger piles are generated because the probability of placing a chip in a pile with a larger number of chips is greater than the probability of placing it in a smaller pile with fewer free spaces with a chip around it. In this way, chips are placed close to others, compacting their grouping, tending to reduce the number of piles over time and not being able to create others by having to place chips close to others. It may happen that a pile splits, but the probability of this happening is very low, since the probability of placing a chip in the positions that are released increases as the pile splits.

The simulation corresponds to a stochastic Random Walk process since all decisions are made randomly with certain rules before doing so. By not having blocked wood piles it is even allowed to remove woods from the large piles, however, because of the probability of placing woods in the contrno of these piles, they tend to grow as their probability is higher than that of placing woods in smaller piles. The rules apply equally throughout the hive and with all termites so that in the long run the rules and their probability of making random decisions tend to generate the same result of clustering the chips over time.
