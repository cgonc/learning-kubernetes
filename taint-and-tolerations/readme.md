````$bash
kubectl taint node node01 spray=mortein:NoSchedule
````

````$xslt
kubectl taint nodes master node-role.kubernetes.io/master:NoSchedule-
````
