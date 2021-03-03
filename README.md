# kubernetes-training

# Install tools
## kubectl

The Kubernetes command-line tool, `kubectl`, allows you to run commands against
Kubernetes clusters. You can use `kubectl` to deploy applications, inspect and
manage cluster resources, and view logs.

See [Install and Set Up `kubectl`](https://kubernetes.io/docs/tasks/tools/install-kubectl/) for
information about how to download and install `kubectl` and set it up for
accessing your cluster.

## minikube

[`minikube`](https://minikube.sigs.k8s.io/) is a tool that lets you run Kubernetes
locally. `minikube` runs a single-node Kubernetes cluster on your personal
computer (including Windows, macOS and Linux PCs) so that you can try out
Kubernetes, or for daily development work.

You can follow the official
[Get Started!](https://minikube.sigs.k8s.io/docs/start/) guide if your focus is
on getting the tool installed.

# Create kubernetes cluster locally
From a terminal with administrator access (but not logged in as root), run:
```
minikube start
```
If minikube fails to start, see the [drivers page](https://minikube.sigs.k8s.io/docs/drivers/) for help setting up a compatible container or virtual-machine manager.

# Interact with your cluster
If you already have kubectl installed, you can now use it to access your shiny new cluster:
```
kubectl get po -A
```