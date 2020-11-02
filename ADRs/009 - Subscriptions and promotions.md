# How will we handle subscriptions and promotions in the system?

## Status
Accepted

## Context
A requirement is to support coupons and promotional pricing and also allow customers to buy a subscription that will mean they can get regular meals.
It is not known if the points of sale can handle any other method of applying discounts (eg. entering promo codes) or if they will simply charge the set price.

## Decision
Both subscriptions and coupons/promotions will be handled by issuing pre-paid cards.  The smart fridge documentation says these are accepted.

## Consequences
We will need to assess 3rd party providers of prepaid cards and choose one.

There will be development required to integrate our website and app with the 3rd party.

We can assume that the distribution and management of these cards will be handled outside of our system.

We will need to handle the linking of a customer account to a pre-paid card.

We may need to review this if we learn about other mechanisms we can use with the points of sale.
