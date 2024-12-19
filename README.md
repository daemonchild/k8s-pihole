# k8s-pihole
Run Pi Hole DNS Filter on Kubernetes


Deploy with:

```
kubectl create namespace pihole
kubectl create -f ./pihole.yaml --namespace="pihole"
kubectl get pod -o=custom-columns=NAME:.metadata.name,STATUS:.status.phase,NODE:.spec.nodeName --namespace="pihole"

```