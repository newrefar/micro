### 网络插件 Flannel

**Kubernetes 集群初始化**

```
kubeadm init --pod-network-cidr=10.244.0.0/16 --apiserver-advertise-address=***.***.***.*** --kubernetes-version=v1.11.1
```

相关文档：[https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/](https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/)

**Flannel 安装**

```
kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/v0.10.0/Documentation/kube-flannel.yml
```