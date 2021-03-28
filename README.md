# microfunctions

[MicroFunctions](https://microFunctions.io/)  is open-source serverless platform bthat lets you deploy small bits of code without having to worry about the underlying infrastructure plumbing. It leverages Kubernetes  resources to provide auto-scaling, API routing, monitoring, troubleshooting and supports every programming language. (Nodejs,Go,python,..).



## Prerequisites

- Kubernetes v1.17+
- Helm 3.1.0

## Install Chart

```console
# Helm
$ helm repo add  microfunctions https://microfunctionsio.github.io/microfunctions-helm
$ helm install my-release microfunctions/microfunctions -n microfunctions --create-namespace 
```

## Uninstall Chart
```console
# Helm
$ helm uninstall [RELEASE_NAME]
```
This removes all the Kubernetes components associated with the chart and deletes the release.

