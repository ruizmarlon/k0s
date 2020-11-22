### Add worker to existing manager(s)

## get token from manager 
```
k0s token create --role=worker > /dev/null 2>&1 &
```
## or to set expiry
```
k0s token create --role=worker --expiry="100h" > /dev/null 2>&1 &
```

## join new worker
```
k0s woker <token here> > 
