# 9. Event-driven microservices architecture

Date: 2020-11-01

## Status

Accepted

## Context

As a result of functional and non-functional requirements ([Requirements](../requirements/Requirements.md), [Architecture Characteristics](../solution-discovery/Architecture\ Characteristics.md)), team came up with the following main qualities Farmacy Food solution should have:
- Availability
- Scalability
- Resiliency
- Elasticity
- Security
- Agility

Separately, architucture team would like to emphasize "Evolvability": Farmacy Food is a perspective startup that has plans to grow, adjust it's business model and exposure to customers. This means that solution should be easy evolvable with company pace.

Consideration points:
- solution should support different architecture characteristics for different parts of the system
- there are syncronious and asychronious flows

## Decision

Event-driven microservices is selected as the target architecture style for Farmacy Food solution

## Consequences

Selected architecture style has the following major trade-offs:
- implemenation cost and complexity
- testability of event-driven asynchronious flows

