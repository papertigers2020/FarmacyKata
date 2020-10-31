# How will we apply user preferences to searches?

## Status
Proposed

## Context
Customers using the website or mobile app will be able to set their preferences about the types of meal they want.  These could be things like "Good for Diabetes" or "Low in fat".  

## Decision
The preferences will be stored in the Profile in the Customer Database.  When a customer logins in to the website their preferences become available to the web and mobile apps.  Their preferences can be automatically configured on the search page as filters so that the user doesn't need to apply them.  The filters will be passed to search endpoint in the General API.
It is expected that all filter options on the search page could be changed by the user, in case they want to see what else is available outside of their preferences.
The reason for this decision is to improve the user experience but also to ensure separation between the Customer API and the General API.

## Consequences
The Web and App UIs will need to be built to store the users preferences locally (cookies/local storage etc.)