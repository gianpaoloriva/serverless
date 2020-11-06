## Create Kubernetes Stack

### Build Docker image
```

https://hub.docker.com/r/lambci/lambda
docker pull lambci/lambda

docker run --rm lambci/lambda:build-python3.8 aws --version
docker run --rm -v "$PWD":/var/task:ro,delegated lambci/lambda:python3.8 lambda_function.lambda_handler


```