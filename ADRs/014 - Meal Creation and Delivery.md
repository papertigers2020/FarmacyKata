# How will the business decide what meals need to be created and delivered to specific locations?
## Status 
Proposed
 ## Context 
Smart fridges need to be topped up with meals in order for business continuity. 
## Decision 
Kitchen API will periodically make a call to the inventory API for the status of the Smart fridge & Kiosk PoS APIs to find out the need for delivery.  It will also call chefTec to get recipes and once prepared, it will be delivered to smart fridges.
## Consequences
There is some estimation & approximation involved here but can be optimised later using Machine learning mentioned in the other ADR.