# k0s
working with k0s

# issues

### coredns will not find the /etc/resolv.conf

It is necessary to change the configmap(cm) and use a dns service like 8.8.8.8 (google dns) 

from:
```
        forward . /etc/resolv.conf
```

to:
```
        forward . 8.8.8.8
```
