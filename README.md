# minikube Installation
minikube setup for k8ts
## What you’ll need
 2 CPUs or more ,
 2GB of free memory ,
 20GB of free disk space ,
 Internet connection
  
## Operating system 
linux
x86-64

## Download binary --
### use Non-root Privileges but having a docker Privileges
```
 curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```
```
 sudo install minikube-linux-amd64 /usr/local/bin/minikube
```
## Start Your cluster --
```
minikube config set driver docker
```
```
minikube start
```
## intrect with your cluster 
```
minikube kubectl -- get po -A
```
## make alias for use kubectl esier
```
echo "alias kubectl='minikube kubectl --'" >>.bashrc

```
## minikube status
```
minikube status
```
## its look like :-
```
ubuntu@ip-172-31-26-155:~$ minikube status
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured
```

