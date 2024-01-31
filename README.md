# Jmeter

Learning performance testing with Jmeter

HW#1
record the following script for Shopizer
- Open home page
- Open category page
- Open product page
- Add to cart
- Checkout
- Proceed to checkout
- Fill order fields
- Submit order(Please use Belgium as a Country)

filter out all requests that seem non required to you in the performance script.
it is important in this task to think about requests that should or should not be left in the script.
I want you to answer the questions "Why is it needed / not needed?"

run a test on 1 user and check the View Results Tree lisener to find out where what information is located, Test different response options in response viewer

HW#2
Record checkout flow for Shopizer
- Open home page
- Open category page
- Open product page
- Add to cart
- Checkout
- Proceed to checkout
- Fill order fields
- Submit order

Parameterize scenario:
- replace domain and similar data with variables in user defined variables
- parameterize end user inputs with jmeter functions
- correlate requests data (using regular expressions or json path)

Jmeter scenario should
1) open random available category from the main page
2) when opening the category page, products for this category should be requested
3) product should be selected from available for this category, the same product should be added to the cart and an order should be made
4) last 2 transactions may fail with a 500th error, this is ok for now, but you can parameterize them anyway and fix as I showed in the lesson with adding a JSR223 post processor to Add to cart request

HW#3
1) register manually (not with a Jmeter) 2-3 users
2) add a login to the script
3) add several (make it as a parameter) different products to the cart. Note: items should be different
4) after opening cart, add  step to delete one of the items in the cart
5) change the quantity of some product and click recalculate
