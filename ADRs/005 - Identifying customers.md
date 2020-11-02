# Credit/debit card details are our only unique identifiers for all customers

## Status
Accepted

## Context
We need to understand which information that we might be able to use to identify customers and their purchase histories, preferences etc

## Decision
We are considering the minimum information that we will be able to collect from customers. In this case, we are assuming that when a customer is making a purchase at a POS as an anonymous customer with no account or subscription, the only information that we will be able to track against the purchase is the credit/debit card that they will use.

## Consequences
We will not be able to track the state of anonymous customers' dietry requirements or health goals. It means we should be able to construct a purchase history for the card used, although it is possible that the card is sometimes used to purchase meals for other people such as family members or friends.  It will also be difficult to track when a customer is issued a new card and understand it is the same customer.
