# microfunctions
<p align="center">
  <a href="https://microfunctions.io" target="blank"><img src="http://www.microfunctions.io/wp-content/uploads/2020/07/New-Project-3.png" width="320" alt="Microfunctions Logo" /></a>
</p>

[MicroFunctions](https://microFunctions.io/) is open-source Kubernetes Native Serverless platform bthat lets you deploy small bits of code without having to worry about the underlying infrastructure plumbing. It leverages Kubernetes  resources to provide auto-scaling, API routing, monitoring, troubleshooting and supports every programming language. (Nodejs,Go,python,..).

- [x] Add Multi Namespace
- [x] Add Multi Cluster (SupportVersions ['v1.17.*', 'v1.16.*', 'v1.17.*','v1.18.*','v1.19.*','v1.20.*'],supportDistributions ['digitalocean','vanilla'])
- [x] Functions API(Https)
- [x] Functions Services
- [x] Functions Cronjob
- [x] Functions Resource Quota
- [x] Functions Autoscale
- [x] Functions Metrics  
- [x] Support Runtime (Python, Node.js, Golang)
- [x] Authorization API (x-apikey-header)
- [ ] Add microFunctions-cli-api 
- [ ] Add Support Cluster Distributions(Aws,GKE,Azure,...)(coming soon)
- [ ] Add Support Runtime(Php,.Net ,java ...) (coming soon)
- [ ] Namespace Resource Quota (coming soon)
- [ ] Dashboard (coming soon)
- [ ] WebApp (coming soon)
- [ ] User types (coming soon)


## How it works
MicroFunctions is a combination of open source tools.
- Kong Ingress Controller implements authentication, transformations, and other functionalities across Kubernetes clusters
- cert-manager controller.  issuing certificates from a variety of sources
- Kubeless Kubernetes-native serverless framework

## Architecture

![MicroFunctions Architecture](https://user-images.githubusercontent.com/67606926/113181595-41921b80-9252-11eb-87b7-4b60112ac99e.png)

## Presentation

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/XhlmzagrtBU/0.jpg)](https://youtu.be/XhlmzagrtBU)

## repositories
[Microfunctions-helm](https://github.com/microfunctionsio/microfunctions-helm)

[Microfunctions-console](https://github.com/microfunctionsio/microfunctions-console)

[Microfunctions-controller](https://github.com/microfunctionsio/microfunctions-controller)

[Microfunctions-cluster](https://github.com/microfunctionsio/microfunctions-cluster)

[Microfunctions-serverless](https://github.com/microfunctionsio/microfunctions-serverless)

[Microfunctions-init](https://github.com/microfunctionsio/microfunctions-init-job)

## Development Setup

Have you found a bug :bug: ? Or maybe you have a nice feature :sparkles: to contribute ? The [CONTRIBUTING guide](https://github.com/microfunctionsio/microfunctions/blob/main/CONTRIBUTING.md) will help you get your development environment ready in minutes.
 

## Prerequisites

- Kubernetes v1.17+
- Helm 3.1.0

## Install Chart

```console
# Helm
$ helm repo add  microfunctions https://microfunctionsio.github.io/microfunctions-helm
$ helm install my-release microfunctions/microfunctions -n microfunctions --create-namespace 
```
[Instal local with Docker Desktop](https://github.com/microfunctionsio/microfunctions/blob/main/Install/install.md)
## Uninstall Chart
```console
# Helm
$ helm uninstall [RELEASE_NAME]
```
This removes all the Kubernetes components associated with the chart and deletes the release.

