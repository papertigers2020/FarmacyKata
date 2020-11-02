# What happens when a fridge malfunctions?

## Status
Accepted

## Context
What happens if a fridge malfunctions and therefore can no longer safely store food?

## Decision
Fridges are managed by a third party API and it is assumed that this API is notified when issues occur. So we do not have to manage the processes around this, but our inventory database will be updated if the status of a smart fridge changes. 

## Consequences
We don't have to manage the smart fridges' status but we will ingest this information so it can be provided to the kitchens.
