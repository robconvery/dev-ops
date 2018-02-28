# dev-ops
devOps notes

## Create ssh key
```
ssh-keygen -t rsa -b 4096 -C "hello-world@example.com" -f id_something
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

## ssh-copy-id
Install on a MAC
```
brew install ssh-copy-id
```

test with
```
which ssh-copy-id
``` 

Using ssh-copy-id
```
ssh-copy-id -i ~/.ssh/id_something \
-o "PubkeyAuthenication no" root@{my-ip-address}
```
