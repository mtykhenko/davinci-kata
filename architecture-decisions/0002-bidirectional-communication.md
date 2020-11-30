# 2. Bidirectional communication with a fridge and kiosk

Date: 2020-10-29

## Status

Superceded by [4. Integration with points of sale](0004-integration-with-points-of-sale.md)

## Context
There are use cases where we need a communication between our system and a fridge/kiosk to be bidirectional. For example applying a coupon during a sale or booking some meal online.<br>
We need to find an approach how to support this communication.

## Decision Drivers
1. A customer should be able to use a smart fridge and a kiosk without account in our system.
2. The user is identified by his/her credit/debit card used to get access to a fridge.
3. Registered user should be able to apply coupons and use promotional pricing.
4. Fridges and kiosks should support online and offline selling including booking of sold meal until it's taken by the owner.
5. We operate with fridges via API of cloud based management system, we may not work with fridges directly.

## Considered Options
### 1. Kiosks and fridges use our software to operate with meals.

#### Pros
1. We fully control whole selling chain and have the freedom to change anything in this chain.
2. We can easily add loyalty flows and online and offline selling since we control the chain.

#### Cons
1. Complex and expensive onboarding process for new fridges and kiosks.
2. Not all fridges support our software.
3. We are responsible for maintenance of software in fridges and kiosks.
4. Additional complexity. We need to balance between security of whole system (that can be compromised by some outdated software on edge device) and availability (let a fridge operate with outdated and not secure software).

### 2. Kiosks and fridges don't use our software to operate with meals.

#### Pros
1. We can add loyalty flows in our system after a purchase is made.
2. Maintenance of fridges and kiosks is not our responsibility.
3. We can add any fridge to our system that cloud based management system supports.

#### Cons
1. We cannot support online selling.
2. Hard to add anything to selling chain since we don't control it. We can work after a purchase when we take a control.

## Decision
Kiosks and fridges use our software to operate with meals.<br>
Rationale is that we have to support both online and offline selling.
