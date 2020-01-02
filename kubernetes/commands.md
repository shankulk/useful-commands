1. List pods
> kubectl get pods

1. List and delete `evicted` pods
> kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod
