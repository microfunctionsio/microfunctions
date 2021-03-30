# microfunctions
<p align="center">
  <a href="https://microfunctions.io" target="blank"><img src="http://www.microfunctions.io/wp-content/uploads/2020/07/New-Project-3.png" width="320" alt="Microfunctions Logo" /></a>
</p>

[MicroFunctions](https://microFunctions.io/)  is open-source serverless platform bthat lets you deploy small bits of code without having to worry about the underlying infrastructure plumbing. It leverages Kubernetes  resources to provide auto-scaling, API routing, monitoring, troubleshooting and supports every programming language. (Nodejs,Go,python,..).

- [x] Add Multi Namespace
- [x] Add Multi Cluster (SupportVersions ['v1.17.*', 'v1.16.*', 'v1.17.*','v1.18.*','v1.19.*','v1.20.*'],supportDistributions ['digitalocean','vanilla'])
- [x] Functions HTTPS
- [x] Functions API
- [x] Functions Cronjob
- [x] Functions Resource Quota
- [x] Functions Autoscale
- [x] Functions Metrics  
- [x] Support for Python, Node.js, Golang
- [x] Authorization API (x-apikey-header)
- [ ] Dashboard (coming soon)
- [ ] webApp (coming soon)
- [ ] User types (coming soon)
- [ ] Add Cluster Distributions(aws,GCE - GKE,Azure,...)

## How it works
MicroFunctions is a combination of open source tools.
- Kong Ingress Controller implements authentication, transformations, and other functionalities across Kubernetes clusters
- cert-manager controller.  issuing certificates from a variety of sources
- Kubeless Kubernetes-native serverless framework
## Architecture

![MicroFunctions Architecture](https://user-images.githubusercontent.com/67606926/113028621-c403d800-918b-11eb-8fdf-58494e4f9e03.png)

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

