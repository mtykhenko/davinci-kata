# 8. Integration between bounded contexts

Date: 2020-11-01

## Status

Accepted

## Context

We're solving the problem of integration between several bounded contexts in a distributed system.
Key required characteristics are following:
- end users oversee availability of selected items near realtime
- support potential business growth: number of customers, POSs, distributors, etc. (scalability)
- system should be easy to maintain and extend, if needed

## Decision

One of the ways to achieve resiliency and scalability is to allow eventual consistency.
Architectural style supporting this model is: event driven architecture (aka, message based architecture)

## Consequences

Although, we understand complexities related to implementation of message based architecture, we think its use is justified in our case