# StatefulSet – Kubernetes

## Overview
StatefulSet is used to manage stateful applications that require
stable network identity and persistent storage.

## Use Case
- Databases (MySQL, PostgreSQL)
- Distributed systems (Kafka, Zookeeper)

## Files
- mysql-headless-service.yaml
- mysql-statefulset.yaml

## Commands Used
kubectl apply -f mysql-headless-service.yaml
kubectl apply -f mysql-statefulset.yaml

kubectl get statefulsets
kubectl get pods
kubectl get pvc

## Verification
kubectl describe statefulset mysql

## Cleanup
kubectl delete -f mysql-statefulset.yaml
kubectl delete -f mysql-headless-service.yaml
