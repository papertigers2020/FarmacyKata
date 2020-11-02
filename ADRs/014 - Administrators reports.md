# How will administrators be able to access sales and other data?

## Status
Accepted

## Context
As with any commercial business there is a requirement for business owners to report on data gathered by the system in order to understand how the business is performing.

## Decision
We will provide an admin interface that admin users can login to in order to access reports on the data and potentially run queries on the data to create new reports.
The Admin interface will use the General API to get the data required for the reports.
This will be part of the main webapp but with a separate UI.

## Consequences
A new interface will need to be built just for admin users.

Authorisation to access this app will need to be built in to the admin user profiles. 
