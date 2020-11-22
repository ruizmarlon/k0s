### Add worker to existing manager(s)

## get token from manager 
```
k0s token create --role=worker
```
## or to set expiry
```
k0s token create --role=worker --expiry="100h"
```

## join new worker
```
k0s woker <token here> > 
