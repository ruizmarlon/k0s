### get amd64 bits
```
wget https://github.com/k0sproject/k0s/releases/download/v0.7.0/k0s-v0.7.0-amd64
mv k0s-v0.7.0-amd64 k0s
chmod +x ./k0s
```

### alternatively get arm64 bits
```
wget https://github.com/k0sproject/k0s/releases/download/v0.7.0/k0s-v0.7.0-arm64
mv k0s-v0.7.0-arm64 k0s
chmod +x ./k0s
```

### create cluster.yaml from default generator
```
./k0s default-config > cluster.yaml
cat cluster.yaml
```
### add san for ip/dns to reach externally
```
vim cluster.yaml
```
### start k0s as background process
```
sudo ./k0s server --enable-worker -c cluster.yaml > /dev/null 2>&1 &
```
### alternatively for arm64
```
export ETCD_UNSUPPORTED_ARCH=arm64
sudo -E ./k0s server -c cluster.yaml
```
### grab kubeconfig
sudo cat /var/lib/k0s/pki/admin.conf > kube.yml

## install `kubectl`
### get kubectl bits
```
curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl"
```
### alternatively grab arm64 bits
```
curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/arm64/kubectl"
```
### make kubectl executabble
```
chmod +x ./kubectl
```
### move binary to your PATH
```
sudo mv ./kubectl /usr/local/bin/kubectl
```
### test install
```
kubectl version --client
```

### test locally
```
export KUBECONFIG=kube.yml
kubectl version
```

### test externally
Change the local to FQDN or IP and add kube.yml to lens



