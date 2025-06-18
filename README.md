# k8s-practice-YT

yaml file to create pod
```ssh
kubectl apply -f pod.yaml
```

yaml file to delete pod
```ssh
kubectl delete -f pod.yaml
```

check diff in old and new file
```ssh
kubectl diff -f pod.yaml
```

run command in pod's container
```ssh
kubectl exec mypod -c bala env
```
mypod --> pod name  <br>
-c bala ---> container name

enter inside container if platform killrcoda
```ssh
kubectl exec -it mypod -- bash
```

otherwise use
```ssh
kubectl exec -it mypod bash
```
