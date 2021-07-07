I
# Install Minikube On Macos 

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64
sudo install minikube-darwin-amd64 /usr/local/bin/minikube
```
# Start Minikube

```
minikube start
```
output

```
 ~ minikube start
😄  minikube v1.21.0 on Darwin 11.4
✨  Automatically selected the hyperkit driver
💾  Downloading driver docker-machine-driver-hyperkit:
    > docker-machine-driver-hyper...: 65 B / 65 B [----------] 100.00% ? p/s 0s
    > docker-machine-driver-hyper...: 10.52 MiB / 10.52 MiB  100.00% 6.86 MiB p
🔑  The 'hyperkit' driver requires elevated permissions. The following commands will be executed:

    $ sudo chown root:wheel /Users/sangam/.minikube/bin/docker-machine-driver-hyperkit 
    $ sudo chmod u+s /Users/sangam/.minikube/bin/docker-machine-driver-hyperkit 


💿  Downloading VM boot image ...
    > minikube-v1.21.0.iso.sha256: 65 B / 65 B [-------------] 100.00% ? p/s 0s
    > minikube-v1.21.0.iso: 243.03 MiB / 243.03 MiB [ 100.00% 21.68 MiB p/s 11s
👍  Starting control plane node minikube in cluster minikube
💾  Downloading Kubernetes v1.20.7 preload ...
    > preloaded-images-k8s-v11-v1...: 492.20 MiB / 492.20 MiB  100.00% 17.23 Mi
🔥  Creating hyperkit VM (CPUs=2, Memory=4000MB, Disk=20000MB) ...
🐳  Preparing Kubernetes v1.20.7 on Docker 20.10.6 ...
    ▪ Generating certificates and keys ...
    ▪ Booting up control plane ...
    ▪ Configuring RBAC rules ...
🔎  Verifying Kubernetes components...
    ▪ Using image gcr.io/k8s-minikube/storage-provisioner:v5
🌟  Enabled addons: storage-provisioner, default-storageclass
🏄  Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default

```

# verify minikube is running

```


➜  ~ kubectl get po -A
NAMESPACE     NAME                               READY   STATUS    RESTARTS   AGE
kube-system   coredns-74ff55c5b-pv5nl            1/1     Running   0          2m48s
kube-system   etcd-minikube                      1/1     Running   0          3m2s
kube-system   kube-apiserver-minikube            1/1     Running   0          3m2s
kube-system   kube-controller-manager-minikube   1/1     Running   0          3m2s
kube-system   kube-proxy-7vrs7                   1/1     Running   0          2m48s
kube-system   kube-scheduler-minikube            1/1     Running   0          3m2s
kube-system   storage-provisioner                1/1     Running   1          3m2s
```

# Install argocd via brew on OSX

```
brew tap argoproj/tap
brew install argoproj/tap/argocd
```
