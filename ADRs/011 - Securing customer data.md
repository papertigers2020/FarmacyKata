# How do we provide security for the Customer data?

## Status
Proposed

## Context
Customer data needs to be stored and accessed securely.

## Decision
Customer data will be stored in a separate database from all other data to provide this separation.  It will also have its own REST API tso we can control the access of the data. 

## Consequences
