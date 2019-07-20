Hackathon question:

Checkout the file RV_Store_Hackathon.pdf

Explanation:
UI -> API Gateway -> Order-api, Product-api
Order-api -> MongoDB
Order simulator -> Every few mins grabs a random name, calls product-api gets a product, create an orders and submit it/save the order in mongo.


# ToDo:

1. Fix the secrets from mongodb deployments. I know it's a No-No.

# How to run


On mac, switch to docker-for-desktop kubernetes cluster and run:

```
kubectl -f apply .
```

# Check the results

```
Go to localhost:30080/
Update the Backend host name to http://localhost:30090/    # Don't forget the / in the end
Click Update.
```

# How to delete the cluster

```
kubectl delete deployments,jobs,services,pods --all
```
