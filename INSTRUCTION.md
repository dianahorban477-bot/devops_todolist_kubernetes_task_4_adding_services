# Instruction for launching, scaling and network testing ToDo application
## 1. Deploying Kubernetes Pods and Services
Run the following commands from the project root directory to create the namespace of names, lauching Pods and setting up networking Services:
```bash
kubectl apply -f .infrastructure/namespace.yml
kubectl apply -f .infrastructure/busybox.yml
kubectl apply -f .infrastructure/todoapp-pod.yml
kubectl apply -f .infrastructure/clusterip-svc.yml
kubectl apply -f .infrastructure/nodeport-svc.yml