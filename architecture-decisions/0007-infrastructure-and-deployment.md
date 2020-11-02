# 7. Infrastructure and deployment

Date: 2020-10-31

## Status

Accepted

## Context

During initial session with a customer deployment to the Cloud was announced as a desired option.
From another side, project budjet is limited which means:
- upfront infrastructure costs are undesired
- infrastructure management should be cheap

## Decision

Solution should be designed for one of major cloud providers
MVP should be based on managed servives as much as possible

## Consequences

MVP solution built based on managed services of some particular cloud provider will result a vendor lock. Change of Cloud provider can require migration efforts in the future