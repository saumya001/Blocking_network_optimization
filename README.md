# Blocking_network_optimization

## What

Commodities are moved over a railway network with a defined origin and destination stations. To minimise the intermediate handlings, multiple commodities are moved as a block (grouped together) from origin to destinations stations which can be different from the actual path. The commodity undergoes re-classification at special stations called nodes and then proceeds further along the path. The railroad blocking problem is to identify this classification plan for all commodities at all nodes in the network. Grouping commodities into blocks allows to minimize the number of switch operations at intermediate nodes, such that, moving costs (= km travelled by each car) and handling costs (= re-classification costs) are kept as low as possible.

## Why to optimize

Switching / Reclassification tasks are time and cost consuming. Each reclassification causes a one day delay in the commodity on average. Furthermore, the classification process is labor and capital intensive because it requires a large number of staff and large amounts of machinery to sort the traffic, as well as the building and maintenance of large terminals to manage the sorting operation.

## Why heuristics

Since the time taken to get optimal solution > 3 hours for some of datasets, heuristics approach are used for faster near optimal results. Two heuristics used are:
>> Linear programming relaxation and fix (LP and Fix)

>> Relaxation induced neighborhood search (RINS) fix

## File structure

1.) 1806_Model_R_V1 - Instance6_MathModel_Optimisation_Run --> Running only with 6 constraints formulated

2.) 1806_Model_R_V1 - Instance6-LP --> With LP Relaxation

3.) 1806_Model_R_V1 - Instance6-LPFix_bothz --> Method1 of matheuristics

4.) 1806_Model_R_V1 - Instance6_FeasibleSol_sk --> Feasible solution for Method 2 of matheuristics

5.) 1806_Model_R_V1 - Instance6-M2_RINS --> RINS run 

## Requirements

The problem is solved using the solver - Gurobi. 
