# How will the business decide what meals need to be created and delivered to specific locations?
## Status 
Accepted
 ## Context 
Smart fridges and Kiosks need to be re-stocked with meals periodically in order to maintain a good selection of meals from which customers can choose.  Some locations may sell more of a specific item than others due to popularity. 
## Decision 
There is a requirement to provide the kitchen with inventory updates periodically.  It is assumed these updates will be used by the kitchen to understand which points of sale are low on specific inventory and they can plan which meals to make and distribute.  
These inventory reports will be provided by allowing kitchen users to login to our administration interface where they can access reports on inventory at all points of sale across the region.
## Consequences
The kitchen staff will need logins for the Admin interface.  It is assumed they would be more likely to request these reports just after meal times to ensure restocking happens before the next mealtime.

The kitchen will need to know the capacity of each point of sale.

There is some estimation & approximation involved here but can be optimised later using Machine learning mentioned in the other ADR.
