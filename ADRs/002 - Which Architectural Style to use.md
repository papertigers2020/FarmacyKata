# Which Architectural Style to use

## Status
Proposed

## Context
We need to select an architectural style for the system

## Decision
A Service Based Architecture will be used, potentially with some Event Based components.  The key factors in this decision were the non-functional requirements for Scalability, Elasticity and Reliability that were derived from the requirements brief.  Scalability is required to allow the business to grow the number of customers, kitchens, and points of sale.  Elasticity is required as there will likely be peaks and troughs of demand throughout the day corresponding to meal times.  Reliability is required to ensure no failures during the order and payment process, and to ensure the website and app are available for customers to use.

A second consideration that helped us choose this style was the need for a low cost architecture style.  The company is a start-up and therefore cannot spend a lot of money upfront on the system.

A final consideration is that a future requirement is to store personal health information for customers.  This would would require a separation of data storage in order to comply with data regulations.

Event based components may be required for elements such as inventory handling.

## Consequences
With the style chosen we can progress with the breaking down of the problem in to services.