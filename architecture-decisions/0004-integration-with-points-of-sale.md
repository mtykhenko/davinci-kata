# 4. Integration with points of sale

Date: 2020-10-30

## Status

Accepted

Supercedes [2. Bidirectional communication with a fridge and kiosk](0002-bidirectional-communication.md)

## Context

Fridges, Kiosks and any future points of sale have an API providing access to inventory, purchage history; allowing process an online purchase order.
Point of sales are not expected to integrate with any external system. Customer has a limited budget and this makes implemetation of changes to point of 
sales not feasible.

## Decision

New Farmacy Food system should be extensible to:
- be able to integrate with APIs of existing point of sales
- support adding new point of sales to network in the future

New system should initiate communiation with point of sales to fetch and submit any required information, drive sales flow.
Data flow will be bi-directional but newly built system will always act as requestor in any interactions.

## Consequences

1. As soon as points of sales cant push any information updates, new system should implemented polling refresh of inventory and sales information
2. Polling intervals should be carefully considered in order to:
- provide required level of data relevance
- avoid excessive load onto point of sales
3. Ordering service should consider potential staleness of inventory information
