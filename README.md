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
```
##### 4. If you use kubernetes Dashboard then add and launch
```bash
# Minikube bundles the Kubernetes Dashboard, allowing you to get easily acclimated to your new environment:
minikube addons enable metrics-server
minikube dashboard 
```
##### 5. If you get any problem related Network / DNS issue or Docker driver issue then run
```bash
❗ Failing to connect to https://registry.k8s.io/
❗ connection refused localhost:8443

Docker driver issue
sudo systemctl restart docker
minikube start --driver=docker
# forcely if above not work
# minikube start --driver=docker --force --alsologtostderr 
``` 


