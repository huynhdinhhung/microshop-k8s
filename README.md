# microshop-k8s

Kubernetes manifests for Microshop Mongo Lab.

## Namespace

microshop

## Services

- MongoDB
- Auth Service
- Product Service
- Gateway
- Frontend

## Apply

kubectl apply -f microshop.yml

## Check

kubectl get all -n microshop
kubectl get pvc -n microshop

## Test

curl http://localhost:32000/health
curl http://localhost:32080/api/health
curl http://localhost:32080/api/products
