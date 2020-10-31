# How will we support SMS functionality and which functionality will we support?

## Status
Proposed

## Context
A number of requirements mentioned the use of SMS in order to provide a method of interacting with customers without access to the website or mobile app.  Possible uses of SMS could be to allow users to text a number to find out what meals are available near them, also to allow a user to receive marketing messages and rate their meals.

## Decision
We will use a 3rd party provider that will enable marketing messages to be sent out to users.  For example letting all users who have a specific health condition know about a new meal suitable for them.
We will not allow users to search for meals near them via SMS message.
We will not allow users to rate their purchases by responding to an SMS message.

## Consequences
We will need to assess 3rd party SMS service providers to choose one with which to integrate.
Work will be required to periodically download our customer records and upload them (just the data needed) to the 3rd party so we can set up marketing SMS messages and target them at specific groups of users.
We will need to investigate the additional functionality not currently supported in the future.