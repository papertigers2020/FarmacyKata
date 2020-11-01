# Where does the customer pay for the meal?

## Status
Proposed

## Context
Can a customer on the website or using the application pay for a meal before they go to collect it? Or do they have to pay when they reach the POS?

## Decision
Customers can only pay for meals at the Point of Sale (Fridge or Kiosk).  As mentioned in ADR005 and ADR006 there is no way to prevent a purchased item being taken by a walk up customer.  
We do not directly communicate with the smart fridges; it is done via an API that the fridges keep in contact with. This system creates problems when considering the synchronicity required to ensure that purchases are not duplicated.

## Consequences
We dont need to handle purchases in the system, that will all be handled by the external systems. 
This will make it easier to design a flow that prevents customers from buying something and then finding it has been removed by another customer when they reach the POS.
