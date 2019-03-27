# XMRig K8s

Mine Monero using leftover resources in a Kubernetes cluster.

```bash
# clone
git clone --recursive https://github.com/brannondorsey/xmrig-k8s
cd xmrig-k8s

# edit the Kubernetes manifest so that you are mining shares to the right pool / address.
$EDITOR k8s.yaml

# launch 9 resource-limited mining pods in the "xmrig" namespace of your cluster
kubectl apply -f k8s.yaml
```
