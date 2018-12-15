kubeadm init --config init.yaml
kubectl taint nodes --all node-role.kubernetes.io/master-

kubeadm join --token <token> <master-ip>:<master-port> --discovery-token-ca-cert-hash sha256:<hash>

kubeadm join 192.168.56.5:6443 --token abcdef.0123456789abcdef --discovery-token-ca-cert-hash sha256:d14fd2c08359ea697a9f23e5e8c742e0744f664e96395e194f20d5bdc394ee67
