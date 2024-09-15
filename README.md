# training-k8s


## install 

### macos-x install hcloud and terraform
```shell
brew install hcloud terraform
```


## cred

### hcloud and terraform cred
```shell
export HCLOUD_TOKEN=$(cat _cred/hcloud_token)
export TF_VAR_hcloud_token=${HCLOUD_TOKEN}
export TF_VAR_ssh_key=$(cat _cred/id_rsa.pub)
```

### generate ssh-key
```shell
ssh-keygen -t rsa -b 4096 -C "training@lab" -f _cred/ssh/id_rsa -q -N ''
```
