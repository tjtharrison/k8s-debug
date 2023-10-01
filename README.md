# k8s-debug

Kubernetes manifests for debug ubuntu pod that can be used to investigate issues with kubernetes cluster.

## Installation

To install the pod, update the namespace / pod details as required and apply the manifest

```bash
kubectl apply -f pod.yaml
```

## Usage

Once the pod is running, you can exec into it and run commands as required

```bash
kubectl exec -it ubuntu -- sh
```

## Cleanup

Before cleaning up, delete the pod

```bash
kubectl delete -f pod.yaml
```

Now revert any changes made to `pod.yaml`.
