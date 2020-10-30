# How will we handle subscriptions and promotions in the system?

## Status
Proposed

## Context
A requirement is to support coupons and promotional pricing and also allow customers to buy a subscription that will mean they can get regular meals.

## Decision
Both subscriptions and coupons/promotions will be handled by issuing pre-paid cards.  The smart fridge documentation says these are accepted.

## Consequences
We can assume that the distribution and management of these cards will be handled outside of our system.
We will need to handle the linking of a customer account to a pre-paid card.
