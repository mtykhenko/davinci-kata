# Non functional requirements or architecture characteristics

## Extensibility
System needs to integrate with 2 different point of sale APIs. And be able to support other vendors in the future.

## Elasticity
System should sustain different usage patterns, inluding spikes of demand caused by promos, some social events, etc. without degradation of performance

## Availability
Our system should be highly available and be accessible 24/7.

## Resiliency
System should be fault tolerant and continue to operate with reduced funtionality in case of outage of certain components. E.g.: in case Fridge Cloud API is down, it should be still possible to place an order and/or buy at Kiosk.

## Cost efficiency
Solution should be cost efficient and should ensure optimal usage of resources at any load.

## Security
All the data should be encrypted at rest and in transit.
Only authenticated users are allowed to access the system.
Financial transactions have to be performed securely.

## Performance
System should support thousands of requests daily, therefore UX operations should take millisecends to complete.