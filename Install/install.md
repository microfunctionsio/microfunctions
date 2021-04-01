
## Prerequisites

- Kubernetes v1.17+
- Helm 3.1.0
## Kubernetes in local  Docker Desktop
[Kubernetes in local the easy way: Docker Desktop (on Mac)](https://medium.com/backbase/kubernetes-in-local-the-easy-way-f8ef2b98be68)



## Install Chart

```console
# Helm
$ helm repo add  microfunctions https://microfunctionsio.github.io/microfunctions-helm
$ helm install microfunctions microfunctions/microfunctions -n microfunctions --create-namespace --values=https://raw.githubusercontent.com/microfunctionsio/microfunctions/main/Install/values-local-ingress.yaml
```
To add a host name, microfunctions.local , with an IP address 127.0.0.1 , add the following line in the /etc/hosts file:

```console
##
# Host Database
#
# localhost is used to configure the loopback interface
# when the system is booting.  Do not change this entry.
##
127.0.0.1	localhost
127.0.0.1 microfunctions.local
```




