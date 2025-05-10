## Hashicorp Consul

## Install Hashicorp Consul in RedHat Openshift
```
helm repo add hashicorp https://helm.releases.hashicorp.com && helm repo update
helm install consul hashicorp/consul \
--namespace consul \
--set global.name=consul \
--set global.openshift.enabled=true
```
