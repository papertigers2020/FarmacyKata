#  How will a customer only be shown meals that are available near to their location?

## Status
Proposed

## Context
When a customer of the application signs up or logs into their app, we need to understand what meals we can present to them as available. Therefore we need to know whether users are allocated a locale that consists of the kitchen and related POS, whether they can set this themselves and whether they can change this locale.  
It is assumed that a locale comprises of a single kitchen and a number of nearby points of sale (fridges or kiosks).

## Decision
A customer's geolocation will be used to determine which locale they are in. This can either be provided by allowing the app to access their phone's gelocation, or by adding an address/location manually.

A customer should be able to change their locale, in case they travel to another location and want to continue using the service.

## Consequences
This affects the meals that a customer will see as available to them. It also affects the locale being requested by our service when running queries for the customer.
If a new kitchen is added to a locale then we will need to split that locale in to 2, with the closest points of sale being assigned to each kitchen. 
