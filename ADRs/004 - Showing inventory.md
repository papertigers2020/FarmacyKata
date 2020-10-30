#  Will customers be allocated and/or be able to choose a "locale" ie the local kitchen/POS?

## Status
Proposed

## Context
When a customer of the application signs up or logs into their app, we need to understand what meals we can present to them as available. Therefore we need to know whether users are allocated a locale that consists of the kitchen and related POS, whether they can set this themselves and whether they can change this locale.

## Decision
A customer's geolocation will be used to determine which locale they are in. This can either be provided by allowing the app to access their phone's gelocation, or by adding an address/location manually.

A customer should be able to change their locale, in case they travel to another location and want to continue using the service.

## Consequences
This affects the meals that a customer will see as available to them. It also affects the locale being requested by our service when running queries for the customer.