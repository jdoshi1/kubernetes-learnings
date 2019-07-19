Hackathon question:

Checkout the file RV_Store_Hackathon.pdf

Explanation:
UI -> API Gateway -> Order-api, Product-api
Order-api -> MongoDB
Order simulator -> Every few mins grabs a random name, calls product-api gets a product, create an orders and submit it/save the order in mongo.

