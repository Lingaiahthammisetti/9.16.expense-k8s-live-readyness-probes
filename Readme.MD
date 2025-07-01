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