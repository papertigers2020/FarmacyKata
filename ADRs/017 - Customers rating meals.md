# How will we handle customers rating meals?

## Status
Accepted

## Context
A requirement is to allow customers to rate meals. This should only be possible if the customer has actually purchased the meal they are rating.

## Decision
After a verified purchase of a meal the system will notify the user (either via in app notification, sms message or email) and ask them to rate the meal they purchased.
Rating information will be stored in the General Database and periodically the meal entry will recalculate its aggregate rating.  This aggregate rating is what will be shown on the meal information and search results pages of the website and app.

## Consequences
We need a mechanism to send emails, sms and in app notifications based on events in the system.
