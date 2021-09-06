# bp Hello World

Nginx image with Hello World page

## CI/CD
CI/CD actions will run on index.html changes with the following actions:
  1. Build and push the Docker image to Docker Hub
  2. Restart the EKS cluster deployment

## Secrets
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- DOCKER_HUB_ACCESS_TOKEN
- DOCKER_HUB_USERNAME
- KUBE_CONFIG_DATA – A base64-encoded kubeconfig file with credentials for Kubernetes to access the cluster. You can get it by running the following command: `cat $HOME/.kube/config | base64`
