## Assignment 4: Discovery

Name: Siddharth Sharma

UnityID: ssharm24

### 1. Scenario 

We are designing a mobile application for convenient grocery shopping. You might be familiar with ordering a takeout from a restaurant, on phone or on web. This is similar, where you specify your grocery order from our mobile application, and the store will keep it ready, for you to pickup. For now, we are assuming a single grocery store (location fixed) and its catalog of products, which is serviced by our app.  These are some of the questions that would help to decide what features and functionality to include in the applicaiton.

### 2. Questions

- How and when would you like to pay for the order? Pay after or before the order? And would you be comfortable with electronic payment from the application? 
- What functionality would help you in browsing product catalog and ordering products? 
- Would you like to contact in-store employees in some ways, to provide special instructions/comments for orders?
- What do you think should happen when you cannot pick up the order? Do you think you'll need to cancel orders, or modify orders after placing them?
- Would you like to save or schedule orders for future?


### 3. Interview Responses:

#### Response 1

- I would like to pay while pickup. Card payment would work - credit card. I would imagine a drive-through where you could drive your car, pay at the counter, and take your order. Smartphone payment options like Apple Pay or Android Pay would also be convenient. Yes, online payment on app would be useful, in case I don't have card.
- One touch adding of items. Like most online marketplaces, browse, search for things, would be some features I would expect. My commonly bought items would be shown or suggested on the side, would be helpful.


- Yes comments on orders, so that if I need something specific, like get a product with extended "use by" date. I would imagine employees could comment or chat too, so that if there is a problem like long queue of cars, I would know in advance.

- If you are late(I would imagine there being a deadline) you should have multiple options - if you can pick on same day or the next day. These options should be in one tap so that I can schedule without entering dates or something complicated.  I think the modification can work as comments if the order is not yet picked up by employee. On wrong orders, I would want a refund, with returning the item on next store visit.  
- I usually don't schedule things very much in advance. But a section like cart, where you could keep adding things, and order once. 

#### Response 2


- I imagine the process in stages. So you order items on the app and then the store fulfills. I should be able to indicate that I am leaving or coming to the store to pickup. At that time I would make the payment and the store would keep my items ready. This process should be quick(within 15-20 minutes) to be convenient, and would depend of the store to implement it properly. Payment should be electronic, i.e. from the app. 
- 2 things could help
  - Suggested items based on past shopping i've done. 
  - product discoverability is difficult - So if I add something - similar products , cheaper alternatives or similar price range should be suggested or be accessible. 
- Would like comments on the order. Also, when order is getting prepared - it should display the employee responsible, and his contact information, so you could call him up, add or delete items at that moment. 
- There should be an option to "Report" in app - damaged products or errors - select from the order. Select the item and report damaged. For pickup time, you should be able to enter time when you can pickup. Then if you are late, an extension can be provided of 1 or 2 hours. If then too I am late, then order should get canceled and refunded.
- An option like Edit and reorder - not only current list, for future orders too - save list. Discount coupons or offers such as buy 2 more, on products, can be in their own section. 


#### Response 3

- Would prefer electronic payment. If there's an option to pay from SquareCash or paypal inside the app so that i don't have to deal with any cards.
- Ability to favorite items. Maybe what's the most popular in each category or ratings of some sort- these could be similar to what amazon have done - also customer reviews can help too, which we cannot get in the normal store.
- Yes there should be an option for comments. But i would keep the human aspect to the minimum. I should be able to do all things inside app, without relying on any particular person.
- There can be delivery option with extra charges. A time limit could be there with if I am late, then order gets automatically canceled.
- Yes many times I buy the same things, so I should access some kind of template of my common orders. If I schedule order there should be some kind of reminder, email notification of some kind, maybe in the app itself.


### 4. 

![img1](file:///home/sid/Pictures/newpipe.png)

The sequence of actions would consist of -:

1. **Login:** The customer would register with his details on the application. He would need to fill payment details, name and contact information. This user account would be used to track transactions and order history.
2. **Option to orde**r - 
   - **New**: Place a new order.
   - **Past**: See your past orders details and items.
   - **Pending**: The order you have placed but haven't picked up.
3. **Modify Pending orders** - Customer can cancel the order or notify the store if he is not able to come in the pickup deadline. He can extend the pickup deadline, or schedule it the next day. He can also cancel the order.
   - **Change the items**: The customer can change the items if the status of order is "Placed" or "Processing". If the order is "Completed", then he cannot modify the contents.
4. **Past orders**: Customer has the option to see past orders and then add those items in the cart. He can then modify those, add, delete, and then place it as a new order.
5. **New order**: Customer proceeds to choose items he wants to buy. The information comes from the store database, and is continually updated while the customer is ordering.
   - This information is displayed in the form of Product categories and Search. By searching the name or brand, he can add things. 
   - He is also shown related products in the categories, in the related section of the app. This is based on his past orders, frequency of ordered items, or items he has marked as favorite.
   - He is shown offers on products and discounts in the product pages as well.
6. **Add pickup details**: The customer adds details when he will be able to pickup the order, accordingly the store fulfills the order. 
7. **Payment**: This is done electronically via the application or if the customer chooses in-store via cash or credit-debit card.
8. **Pickup**: The customer gets a order number issued when he chooses the payment. He then goes to the store and gives the order number to get his order.



### 5.

Alternate sequence of actions for things that could go wrong:

- **Payment declined** - the store emails the customer as to the reason why the payment was declined. In this case the order is saved for reordering later. Alternate ways of ordering can be presented later in the app.
- **Catalog not up to date** - Product not available - If the customer orders something which is not available in the store, (but it was in the catalog for ordering), then he gets notified of this error by email or app notification. Then he is provided the full refund, and the option to include or notify the item when it is back in stock.
- **Damaged goods** - Frozen Food gone bad - items like ice cream or cakes, when kept extended period of time outside, which can happen during delayed pickup. In this case the customer can return the item, and get a new one, or get a refund.
- **Wrong order** - If the order customer took is not the order he placed. In this case, the store offers to replace the order, and the customer needs to return the previous order. The status of the order could "Pending" until it's not completed.
- **Canceled order** - In this case, the customer is offered full refund.
- **Delayed pickup** - In this case, if the deadline for pickup is over, and the customer has not indicated for extension from the app (to pick up the day after), then the order gets canceled, and customer gets refund.

### 6.

Various Information involved in this process:

- **Store Database** which contains - customer information like name, address, contact details, payment details. This would get created in the app (at the time of account registration), and then used for order processing.
- **Store Database - product catalog** - The catalog would need to be synced between the app and the server. When the customer orders an item, it should reflect in the catalog, to avoid being bought by in store customers. 
- **Order number** - the order would be placed from the application to the server of store, and would translate into a order number for the store to fulfill. This order number would be the primary identification between customer and the store. The customer would show the order no, and the store would get him the order.
- **Status of order** -  When the order is placed the status to the store is "Pending". When employee is fulfilling the pending order - the status changes to "Processing". When order is ready, the status changes to "Ready", which then prompts the customer to pickup from the store. When the pickup is complete the status changes to "Completed".