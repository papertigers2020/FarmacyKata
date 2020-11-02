# How do we handle the expiry of meals in the fridges? 
## Status 
Accepted

 ## Context 
It is important NFR that the business is safe for customers to use. It would not reflect well on the company if a customer bought a meal that was out of date.  A meal that is expired should not be able to be purchased. 

## Decision 
It is assumed the expiry date is part of the data held on the RFID chip on each item.  This expiry date will be part of the inventory information returned by the smart fridge and kiosk apis.  Using this date we can ensure that we dont show expired items on the website or app.

The distributor that delivers meals to points of sale will remove expired items.  There is an opportunity here for the distributor to donate the expired meals to charity.

## Consequences
The removal of expired items from points of sale will be handled entirely by the distributor.

There is a machine learning opportunity here to reduce wastage (see ADR012)
