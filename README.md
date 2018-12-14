kubeadm init --config init.yaml
kubectl taint nodes --all node-role.kubernetes.io/master-

## start kubelet

``` sh
swapoff -a
systemctl start kubelet
```