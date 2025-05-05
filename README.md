# k8-cluster-labs
This repository contains instructions to create kubernetes cluster using kind and docker desktop

## Docker Desktop - Enable K8's cluster
1. Install Docker desktop following instructions mentioned https://docs.docker.com/desktop/setup/install/mac-install/
2. Enable Kubernetes cluster Settings --> Kubernetes --> Enable


## Kind Create K8's cluster
1. Install Kind binary by following instructions mentioned https://kind.sigs.k8s.io/docs/user/quick-start/#installing-from-release-binaries
2. kind create cluster --name devops-cluster  --config multi-node.yaml

## Useful Docker commands
docker run -d --name my-container my-image

docker run -d --name vindocker nginx

docker inspect

docker exec -it e7d63d0b38cb bash

docker rm -f e7d63d0b38cb        (Force fully remove, no need to stop)

docker stop <containerid> && docker rm <containerid>     (Stop and remove container)
