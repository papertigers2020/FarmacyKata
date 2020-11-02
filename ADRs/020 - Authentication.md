# How will we handle authentication of users?

## Status
Accepted

## Context
We need to authenticate users of the website and mobile app when they want to login.   

## Decision
We will use a 3rd party OpenID provider to enable this.  There are many providers such as Auth0 who provide this mechanism.

## Consequences
We will need to assess the 3rd party providers and choose one.

There will be work to integrate our website and app with the provider.

We will need to link the OpenID user with the users in our customer database.
