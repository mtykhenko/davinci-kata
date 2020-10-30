# Selling offline and online in a fridge and kiosk

## Status

Proposed

## Context
Our customers should be able to buy some meals online and choose a proper fridge or kiosk, where they will grab meals. Also our customers should be able to buy meals directly in a fridge and kiosk.
There should be an approach to support both ways of selling.

## Decision Drivers
1. Fridges and kiosks use our software and we control whole selling chain there.

## Considered Options
### 1. Book meal online and release it only to the owner offline.
For example, bar code is marked as booked and can be released only to the owner.
Kiosk employee or a fridge scans bar code during buying and see that the item is booked. Customer should authenticate himself/herself to recieve a meal.

#### Pros
1. Execution process is simple.
2. Sold meal will always wait for an owner in a fridge or kiosk.

#### Cons
1. Increased complixity to minimize duration of meal locking or to apply non-locking approach while online transaction is happening.
2. When/if amount of sales will be high enough, our system will spend lots of time on achiving consistency of orders.

### 2. Operate on prediction of demand, don't book anything.
Fridges and kiosks are refilled regularly. Online orders are made at some point of time in future.<br>
Refillment schedule is based on online orders and usual demand.

#### Pros
1. Execution process is simple.
2. Great performance on high load. System can concentrate on serving customer demands and don't work on meeting consistency between orders.

#### Cons
1. Collitions are rare but possible. During exceptional events (e.g. conference near some fridge will lead to epmty fridge in minutes) planned online bookings won't be handled in time.
2. Sophisticated prediction model.

## Decision
Operate on prediction of demand, don't book anything.<br>
Rationale is that we expect high load on ordering system in pick times for the following reasons and this option handles it better:
- Big disproportion between the number of point of sales and customers (dozens of automated fridges and representative run kiosks, thousands of customers).
- Customers usually buy food 3 times per day during the same time intervals (we operate in a single time zone).