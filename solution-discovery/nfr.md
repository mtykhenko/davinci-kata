# Non functional requirements or architecture characteristics

## Security
We have many points of sale that is hard to control.

## Elasticity
Customers usually buy food 3 times per day during the same time intervals (we operate in a single time zone). So ordering components should support higher load in peak times.

## Availability
Our system should be highly available but only in peak times. It's fine if we do maintenance jobs while majority of customers sleaps.

## Resilience
Our system should support online selling when integrations with external systems are not operational.