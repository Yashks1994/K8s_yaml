# K8s_yaml
This Repo container all template yaml of various Kubernetes resources

The yaml are the declarative way of yaml file.

Below are the Imperative way to create a K8s resource.

### Pod
```
kubectl run nginx --image=nginx --restart=Never
```

### Deployment
```
kubectl create deployment --image=nginx nginx
```
To scale up the replicas-
```
kubectl scale --replicas=3 deployment/nginx
```

### Service
To expose a pod nginx service
```
kubectl expose pod nginx --port=80 --name redis-service
```

To expose a deployment service to NodePort
```
kubectl expose deployment nginx --port=80 --type=NodePort --name nginx
```
