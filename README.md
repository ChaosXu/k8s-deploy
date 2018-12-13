kubeadm init --config init.yaml
kubectl taint nodes --all node-role.kubernetes.io/master-