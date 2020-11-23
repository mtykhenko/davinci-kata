# Requirements Summary

## About the company

Farmacy Food is a tech-enabled healthy food startup that takes the “Let food be thy medicine” quote literally and creates tasty meals around peoples’ dietary needs and active lifestyles to support their overall well-being. Their mission is to make health and wellness radically affordable and accessible.

Founder: Kwaku Osei

## Challenge

A “ghost kitchen” needs a system to allow users to have visibility of what items are available, purchase, and pick up items at any one of their points of sale.

## Functional Requirements

### Immediate

-	Must integrate with 3rd party smart fridges to obtain inventory and purchase activity
-	Smart Fridges Produce item inventory levels and purchases. The smart fridges have a cloud based management system that handles communication with the Smart Fridge so obtaining this data would be through an API.
-   Must integrate with point of sale system at kiosks
-	The Kiosk is a sublet space inside another business where we will sell our product but have an employee handle the transactions through a point of sale. The same data should be accessible through the POS systems API’s.
-   Mobile and Web accessible
-	Support providing feedback on items of verified purchases and in app surveys
-	Accept coupons and promotional pricing
-	Send inventory updates to central kitchen

### Long Term

-	Harvest data to provide personalized recommendations based on users health goals, purchase history, and item ratings

## Non-Functional Requirements

#### Extensibility
System should have the possibility to integrate with more POS APIs and allow multiple vendors to offer items through points of sale

#### Elasticity
System should sustain different usage patterns, including spikes of demand caused by promos, social events, etc. without degradation of performance

#### Scalability
System should be scalable and be able to handle increasing usage with the expansion of business.

#### Availability
System should be highly available and be accessible 24/7.

#### Resiliency
System should be fault-tolerant and continue to operate with reduced functionality in case of outage of certain components. E.g.: in case Fridge Cloud API is down, it should be still possible to place an order and/or buy at Kiosk.

#### Cost efficiency
Solution should be cost-efficient and should ensure optimal usage of resources at any load.

#### Security
All the data should be encrypted at rest and in transit.
Only authenticated users are allowed to access the system.
Financial transactions have to be performed securely.

#### Performance
System should support thousands of requests daily, therefore UX operations should take milliseconds to complete.


## Additional Information

#### Smart Fridge
-   Smartfridges provide a “Grab & Go” option
-   Customers will be able to access with their debit/credit card
-   Customers can order online and effortlessly walk down to pick up their meal

Source : [Farmacy Food Smartfridge Apt Brief](https://github.com/mtykhenko/davinci-kata/blob/master/requirements/Farmacy%20Food%20Smartfridge%20Apt%20Brief.pdf)
         <br/>[Byte Technology Fridges - How it Works](https://bytetechnology.co/#how-it-works)
         
#### Point of Sale Application

POS Application - [Toast POS](https://pos.toasttab.com)

#### Administration

Accounting : [Quickbooks](quickbooks.intuit.com)
<br/>Inventory management, Recipe, Nutrition Analysis : [Cheftec](https://www.cheftec.com/)


