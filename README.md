* Liveness Probe and Readiness Probe are used in Kubernetes to monitor the health and availability of containers:
    * Liveness Probe checks if the container is alive. If it fails, Kubernetes automatically restarts the container.
    👉 Purpose: Detect and recover from application crashes or hangs.

    * Readiness Probe checks if the container is ready to handle traffic. If it fails, the container is removed from the load balancer.
    👉 Purpose: Prevent sending requests to an unready or initializing service.
Both help ensure high availability and smooth operation of applications in a Kubernetes cluster.





# How to create and delete all pods?
```
kubectl apply -f namespace.yaml
```
```
kubectl apply -f mysql/manifest.yaml
```
```
kubectl apply -f backend/manifest.yaml
```
```
kubectl apply -f frontend/manifest.yaml
```
```
kubectl apply -f debug/manifest.yaml
```

```
kubectl delete pods --all -n your-namespace
```
* This is classic load balancer:
```
http://afc79b680d5f34a1694fae92ec7cf3cc-617678930.us-east-1.elb.amazonaws.com

```