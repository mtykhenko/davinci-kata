# Sequence diagram

## Inventory/Purchase updates flow
!["Component diagram"](./images/us_purchase-inventory_feed_flow.png)
### Quick Summary
Flow starts from retrieving data (inventory state,purchases) from external point of sale api (fridge,kiosk). _**`[navigation elements 1,2,3,4]`**_  
Received data is transformed to standardised format that is known to Farmacy Food System. _**`[navigation element 6]`**_  
Data flow is distributed into two directions _**`[navigation elements 7,8,9]`**_
 - notify a kitchen with inventory and purchase updates _**`[navigation elements 10]`**_
 - save current state to inventory database, for further search usage _**`[navigation elements 11]`**_
##Order processing flow
