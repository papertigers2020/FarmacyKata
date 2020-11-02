# Will we support delivery of meals to subscribers homes?

## Status
Accepted

## Context
It was mentioned in the brief that there is a desire to let subscribers get meals delivered to their homes.

## Decision
In this first iteration of the system we will not support subscribers ordering specific meals and getting them delivered to their home.
The main reason for this is to keep the system simple to begin with. We would need to allow preordering of meals that are not yet made or distributed (see ADR005). Kitchens would need to know if they had the ingredients to make all possible meals.

## Consequences
This will need to be added to the architecture at a later date.  
