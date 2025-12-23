# DaemonSet – Kubernetes

## Overview
A DaemonSet ensures that a copy of a Pod runs on every node in the cluster.
It is mainly used for node-level services.

## Use Case
- Monitoring agents (Node Exporter)
- Log collectors
- Security agents

## Files
- node-exporter-daemonset.yaml

## Commands Used
kubectl apply -f node-exporter-daemonset.yaml

kubectl get daemonsets
kubectl get pods -o wide

kubectl describe daemonset node-exporter

## Cleanup
kubectl delete -f node-exporter-daemonset.yaml
