# Devtopia

<img src="https://is1-ssl.mzstatic.com/image/thumb/Podcasts211/v4/cf/88/5b/cf885b65-d9d6-a2cc-0bb7-37b83bc1384e/mza_7921343945018474712.jpg/250x250bb.jpg">

A generic development environment for remote development.

## Developer Guide

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

Or, you may use the [GitHub Codespaces](https://github.com/codespaces) instead of Visual Studio Code running on your local machine.

### Adding new dependencies to the development environment

You may use `devbox add` command to add pkgs from `https://www.nixhub.io/`.  
Or, checkout `taskfiles/_env.yml` and make changes as needed.

### Running Containers

**Docker** should be already up and running. You may use `docker` or `docker-compose` commands to manage the containers.

**Minikube** can be started using `task k8s:up` command. This will start a minikube cluster and create tunnel to access the services with type `LoadBalancer`.
