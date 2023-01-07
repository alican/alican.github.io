# Forward a local port to a port on the Pod 

```bash
kubectl port-forward service/app 8080:8080
```



This will run new test pod and give you `sh` within that pod:

```bash
kubectl run -it --rm test --image=busybox --restart=Never -- sh
```
