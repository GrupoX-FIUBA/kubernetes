# Kubernetes setup

Here are the kubernetes manifests to setup the cluster.

## Instructions

1. Install [kubectl](https://kubernetes.io/docs/tasks/tools/#kubectl).
2. Download the kubernetes config file and paste it in `~/.kube/config`.
3. Apply the files in `manifest` in order (`kubectl apply -f manifest/NN-XYZ.yml`).

> Note: In case you need to replace some values with env vars (e.g. in 02-postgres-deployment.yml), you can do `cat manifest/NN-XYZ.yml | envsubst | kubectl apply -f -`.
