# How do we provide security for the Customer data?

## Status
Accepted

## Context
Customer data needs to be stored and accessed securely.  There is potentially a future requirement for supporting the storage of medical information about customers, this may mean complying initially with HIPAA for USA.  Rollout to other countries may have different data handling requirements.  

## Decision
Customer data will be stored in a separate database from all other data to provide this separation.  It will also have its own REST API so we can control the access of the data. 

## Consequences
An additional Database and REST API will be added to the architecture
