- List pods
> ```kubectl get pods```

- List and delete `evicted` pods
> ```kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod```

- List and delete pods with specific status (`Pending`, `Running`, `Unknown`, `Succeeded`, `Failed`)
> ```kubectl -n default delete pods --field-selector=status.phase=Pending|Running|Failed|Succeeded|Unknown```

- Telepresence Swap Deployment
> ```telepresence --swap-deployment <deployment_name>:<container_name> --env-json telepresence.json```

- Set Environment Variable
> ```kubectl set env deployment/<deployment_name> REPLAY_ENABLED='True'```
