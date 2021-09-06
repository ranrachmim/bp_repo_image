# bp_repo_image

nginx image with Hello World page

## CI/CD
CI/CD actions will run on index.html changes with the following actions:
  1. Build and push the Docker image to Docker Hub
  2. Restart the EKS cluster deployment
