# Horizontal Pod Autoscaler (HPA)

## Overview
HPA automatically scales the number of pods based on resource utilization
such as CPU or memory.

## Prerequisites
- Metrics Server installed

## Files
- app-hpa.yaml

## Commands Used
kubectl apply -f app-hpa.yaml

kubectl get hpa
kubectl describe hpa app-hpa

kubectl top pods
kubectl top nodes

## Cleanup
kubectl delete -f app-hpa.yaml
