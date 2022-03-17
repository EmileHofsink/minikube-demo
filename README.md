# minikube-demo
A demo of minikube to show how to utilise kubectl and kubernetes in a local development environment

## Installation

- To Install (w/ Brew :beer: ):

```brew install minikube```

- To Install (w/ Chocolatey :chocolate_bar: ):

```choco install minikube```

(Note: You’ll need a form of container environment like Docker, containerd or Podman to use Minikube)

## Running

- Start a cluster by running:

```minikube start```

- Access the Kubernetes dashboard running within the minikube cluster:

```minikube dashboard```

- Once started, you can interact with your cluster using kubectl, just like any other Kubernetes cluster. For instance, starting a server:

```kubectl create deployment nginx --image=nginx```

- Exposing a service as a NodePort

```kubectl expose deployment nginx --type=NodePort --port=8080```

- minikube makes it easy to open this exposed endpoint in your browser:

```minikube service nginx```
