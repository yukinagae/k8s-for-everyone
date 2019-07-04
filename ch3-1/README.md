# Usage

deployment

```bash
$ kubectl apply -f deployment.yaml
$ kubectl get pods
NAME                               READY     STATUS    RESTARTS   AGE
nginx-deployment-c97df9bdd-t8zc6   1/1       Running   0          9m
nginx-deployment-c97df9bdd-wzlvt   1/1       Running   0          9m
nginx-deployment-c97df9bdd-xsq9x   1/1       Running   0          9m
```

service

```bash
$ kubectl apply -f service.yaml
$ kubectl get services
NAME            TYPE           CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
kubernetes      ClusterIP      10.96.0.1       <none>        443/TCP          22h
nginx-service   LoadBalancer   10.109.111.56   localhost     8080:30398/TCP   43s
```
