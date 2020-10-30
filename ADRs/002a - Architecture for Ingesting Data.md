
# ADR 2a. Architecture for Ingesting Data

## Status

Proposed

## Context

The system has to ingest information about purchases and inventory updates
from different external sources and store that information.

## Decision

We will create a set of modules for pulling or listening events from the external sources.
One listener/poller from each kind of external source. Those readers will translate external
sources information or events to standardized system domain events that will be published
on a message broker topic.

A set of functionally cohesive modules will register to the topic and listen for those events
asynchronously for  updating the data storage with relevant information. In the case of a
failure processing one event the event will be retried a number of times and in the case of
a continuous failure will be sent to a dead letter queue that will allow to retry it later.

## Consequences

Creating specialized modules for interacting with every kind of device makes it easier to
add more devices without changing existing modules. The topic based communication will allow us
to integrate new readers and processors. Taking into account the business case that kind of
evolution is expected.

The asynchronous event based architecture will provide fault tolerance critical functionality
of ingesting data. This solution will escalate in order to support an increased number of devices
and customers and events, providing elasticity as well for coping with peaks on meals purchases and operation.

This solution is much more complex than a simple synchronous request based architecture and typically
the testing and implementation will require a bigger effort. But we understand that the kind of events
we are going to support does not have complex workflows and they are well defined and easy to test.
