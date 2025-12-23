# Ingress – Kubernetes

## Overview
Ingress provides HTTP/HTTPS routing to services inside the Kubernetes cluster
using host-based or path-based rules.

## Prerequisites
- Ingress Controller (NGINX)

## Use Case
- Exposing applications externally
- Path-based routing
- SSL termination

## Files
- app-ingress.yaml

## Commands Used
kubectl apply -f app-ingress.yaml

kubectl get ingress
kubectl describe ingress app-ingress

## Test Access
Add host entry in /etc/hosts:
<node-ip> myapp.local

## Cleanup
kubectl delete -f app-ingress.yaml
