kubectl apply -f deployment-v1.yaml
# update the service.yaml to point to version: v1
kubectl apply -f service.yaml
kubectl apply -f deployment-v2.yaml
# update the service.yaml version:v2
kubectl apply -f service.yaml
