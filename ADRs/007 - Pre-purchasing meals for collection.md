# Can a customer pay for an item through the app/online before collecting it?

## Status
Proposed

## Context
Can a customer on the website or using the application pay for a meal before they go to collect it? Or do they have to pay when they reach the POS?

## Decision
Customers can only pay for meals once they have reached the POS and collected it.
This is because allowing people to pay for items before collecting means that there must be a way of preventing others from purchasing the meals they have paid for. We do not directly communicate with the smart fridges; it is done via an API that the fridges keep in contact with. This system creates problems when considering the synchronicity required to ensure that purchases are not duplicated.

## Consequences
This will make it easier to design a flow that prevents customers from buying something and then finding it has been removed by another customer when they reach the POS.