# Overview
A TeKanAid Academy Playground to practice Kubernetes skills.

## Instructions

1. You will get access to a Linux terminal with `kubectl`, `helm`, `k9s`, `kubectx`, and `kubens` already installed.
2. A Minikube instance will automatically start, this takes about 5 minutes so please be patient!
3. I've also included a list of aliases to use:
- alias k="kubectl"
- alias kga="kubectl get all"
- alias kgn="kubectl get all --all-namespaces"
- alias kdel="kubectl delete"
- alias kd="kubectl describe"
- alias kg="kubectl get"

## k8s demos 

```
kubectl apply -f yamls/deployment.yaml
kubectl apply -f yamls/service.yaml 
kubectl get pods --all-namespaces
kubectl get svc --all-namespaces
minikube service nginx-service
minikube ip

kubectl describe pod <pod-name> -n <namespace>
kubectl top pod nginx-deployment-688dc88fd-4ptff -n default
```