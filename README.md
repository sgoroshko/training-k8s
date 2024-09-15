# training-k8s


## install 

### macos-x install hcloud and terraform
```shell
brew install hcloud terraform
```


## cred

### hcloud and terraform cred
```shell
export HCLOUD_TOKEN=$(cat priv/hcloud_token)
export TF_VAR_hcloud_token=${HCLOUD_TOKEN}
export TF_VAR_ssh_key=$(cat priv/id_rsa.pub)
```

### generate ssh-key
```shell
ssh-keygen -t rsa -b 4096 -C "training@lab" -f priv/ssh/id_rsa -q -N ''
```
