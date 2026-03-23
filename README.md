# kubernetes_setup
### Minikube (Local / Beginner)
* Learning Kubernetes
* Local testing
* No cloud needed

##### 1. According to my system Operating system (Linux), Architecture(x86-64), Release type (stable) and Installer type (Debain Pakage)__
You can visit minikube start webpage to install according to your system.__
```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
sudo dpkg -i minikube_latest_amd64.deb
```
##### 2. Start your cluster
```bash
minikube start
```
##### 3. Interact with your cluster
```bash
kubectl get po -A
or
# minikube kubectl -- get po -A
# Minikube bundles the Kubernetes Dashboard, allowing you to get easily acclimated to your new environment:
# minikube dashboard 
```

