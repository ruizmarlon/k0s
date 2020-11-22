## Add worker to existing manager(s)

### get token from manager 
```
k0s token create --role=worker
```
### or to set expiry
```
k0s token create --role=worker --expiry="100h" 
```

### join new worker
```
k0s worker <token here> > /dev/null 2>&1 &
```
### check to see if node is ready
```
kubectl get nodes
NAME              STATUS   ROLES    AGE   VERSION
ip-172-14-11-1    Ready    <none>   1m    v1.19.3
```
