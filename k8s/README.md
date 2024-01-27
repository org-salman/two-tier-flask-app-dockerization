# How to setup two-tier application deployment on kubernetes cluster
## First setup kubernetes kubeadm cluster
Use this repository to setup kubeadm https://github.com/org-salman/two-tier-flask-app-dockerization.git

## SetUp
- First clone the code to your machine
```bash
git clone https://github.com/org-salman/two-tier-flask-app-dockerization.git
```
- Move to k8s directory
```bash
cd two-tier-flask-app/k8s
```
- Now, execute below commands one by one
```bash
kubectl apply -f two-tier-flaskapp-deployment.yml
```
```bash
kubectl apply -f two-tier-flaskapp-deployment-svc.yml
```
```bash
kubectl apply -f mysql-deployment.yml
```
```bash
kubectl apply -f mysql-deployment-svc.yml
```
```bash
kubectl apply -f mysql-pv.yml
```
```bash
kubectl apply -f mysql-pvc.yml
```
