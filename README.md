# ballerina-cloud-demo
Demo code to show capabilities of ballerina with docker and kubernetes

## Prerequisites
### Mac
- Docker for Mac - https://docs.docker.com/docker-for-mac/install/.   
- `curl` command tool. Execute `brew install curl` to install with `brew`.  

### Windows
- Docker for Windows - https://hub.docker.com/editions/community/docker-ce-desktop-windows.
- Enable "Expose daemon on tcp://localhost:2375 without TLS" in Docker for Windows settings as follows:
![Expose daemon on tcp://localhost:2375 without TLS](images/docker-localhost-windows.png "localhost daemon")
- Postman or any other REST API Client - https://www.getpostman.com/downloads/.

### Ubuntu/Linux
- Docker - https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04. Note: Make sure you run 'Step 2' as well.
- Minikube for Kubernetes - https://kubernetes.io/docs/tasks/tools/install-minikube/.
- `curl` command tool.

## Demo 1
[See Source Code and Artifacts](demo-1)

In this demo we will be writing a "Hello World" Ballerina service and then run it on Docker.

We will write a Ballerina service which responds "Hello, World!".

## Demo 2
[See Source Code and Artifacts](demo-2)

In this demo we will be creating a Docker image for the service using `@docker` annotation(s).

## Demo 3
[See Source Code and Artifacts](demo-3)

In this demo we will be deploying the Docker image generate earlier(from Demo 2) to Kubernetes.

## Demo 4
[See Source Code and Artifacts](demo-4)

In this demo we will be deploying the Docker image generate earlier(from Demo 2) to Kubernetes using `@kubernetes` annotation.
