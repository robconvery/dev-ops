# dev-ops
devOps notes

## Create ssh key
```
ssh-keygen -t rsa -b 4096 -C "robconvery@me.com" -f id_something
```
## Add key to authorised_keys

copy local public key
```
cat id_something.pub | pbcopy 
```

add to authorised_keys
```
nano authorized_keys
```
...and paste in public key   
