## Create Deployment with kubectl
```
kubectl create deployment nginx --image=nginx:latest
```

## Make the application accessible from the internet
```
kubectl expose deployment nginx --port 80 --type NodePort

kubectl get service nginx # get the port of the external service

kubectl get nodes -o wide # get one IP address
```