# Do we support the preordering of meals not presently at a POS?

## Status
Proposed

## Context
If a meal is not available at a Point of Sale (kiosk, smart fridge etc), can a customer preorder a meal to be delivered to that point of sale at a later time?

## Decision
This functionality is not supported for now because of the complexity it will add to the flow we already have. 

From researching the smart fridge capabilities it does not appear to be possible to put an item in a fridge for a specific customer to collect (eg. in the style of an Amazon Locker) as the shelves of the fridge are open and any walk up customer could purchase the item by removing it from the fridge before the customer who placed the order could collect it.

Adding this functionality would also have meant telling the kitchen for the customers' locale that it needs to create the meal for a specific location. This causes complexity because it would take away some of the control a kitchen has over the meals that it produces. It would also mean that the application would need to understand the capability of a kitchen to produce that meal before allowing a customer to preorder it.

## Consequences
This decision will make it easier for kitchens to control the inventory that it provides and effectively removes a workflow from the overall system.
It also means that customers will be restricted to buying only what is already available in their locale.
