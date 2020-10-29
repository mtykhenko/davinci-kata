# Farmacy Food Scenarios

## Customer Actions
- [CA1] Use system via web browser.
- [CA2] Use system via mobile phone.
- [CA3] Login via Facebook,Apple,etc.
- [CA4] Search by different criteria: location,nutritients.
- [CA5] Search meals in nearest Kiosks. 
- [CA6] Search meals in nearest Fridges. --> (swipe credit card,open fridge,take meal)
- [CA7] [TBD] Buy meal via credit card and pickup in Kiosk.
- [CA8] [TBD] Buy meal via credit card that is present in Fridge.
- [CA9] Apply coupon while paying for order.
- [CA10] Apply subscription for meals delivery.
- [CA11] Choose to participate in available loyalty program.
- [CA12] [NICE TO HAVE] Can register using transaction id from POS.
- [CA13] Provide feedback on items of verified purchases 
- [CA14] Provide feedback on items in app surveys

## POS Person Actions
- [PPA1] Should accept code from application (confirmation that order completed) and give order to customer.
- [PPA2] Check local inventory, place order, complete payment , issue receipt and meal.

## Farmasy Food Manager Actions
- [MA1] Add meals and/or ingredients list into system.
- [MA2] [NICE TO HAVE] View sales history in all kiosks,fridges
- [MA3] View meals demand.
- [MA4] View inventory in all fridges,kiosks.
- [MA5] Provide meals plan for kitchen (Get meals demand, base on consumption and orders from customers)
- [MA6] Generate regular delivery plan
- [MA7] Analysis of customer feedback 
- [MA8] Create surveys and send to customers
##  Kitchen Actions
- [KA1] Get meals plan regularly.

## Delivery Service (Company) Actions
- [DA1] Get delivery plan (from what Kitchen to delivery meals,location to deliver, and quantity).
- [Assumption] We will use POS and Fridge api to provide delivery confirmation/fridge inventory update.

## System Actions
- [SA1] Get information about purchases from fridges (https://bytetechnology.co/#how-it-works)
- [SA2] Get available inventory from fridges (https://bytetechnology.co/#how-it-works)
- [Assumption] We assume that we integrate only with one POS system toasttab.
- [SA3] Get information about purchases from kiosks POS (https://pos.toasttab.com)
- [SA4] Get available inventory from kiosks POS (https://pos.toasttab.com)
- [SA5] [TBD] Mark meals as bought in kiost POS online.
- [SA6] [TBD] Mark product as bought in fridge online.
- [SA7] Charge customer when its order was confirmed. 
- [SA8] Notify kitchen when there is need for some meal in certain location - **To discuss with Uolodymyr**.

## Questions
1. What is priority of customers: customer that bought online vs that comes phisically.

## Internal Questions
- Think how to buy online and offline in a fridge/pos ([SA5], [SA6]).
- Think about 2 directional connection between our system and fridge/pos. For example discounts while buying in a fridge. NOTE: we don't control whole chain.
