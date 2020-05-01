Ingress Setup
------------------

create a namespace as ingress controller
$ kubectl create namespace ingress-space

create a configmap in ingress-space namespace named nginx-configuration
$ kubectl create configmap nginx-configuration --namespace ingress-space

create a service account for nginx ingress controller named ingress-serviceaccount
$ kubectl create serviceaccount ingress-serviceaccount --namespace ingress-space

create a role named ingress-role
$ kubectl apply -f ingress-role.yaml

create a role binding named ingress-role-binding
$ kubectl apply -f ingress-role-binding.yaml

create a cluster role named ingress-clusterrole
$ kubectl apply -f ingress-clusterrole.yaml

create a cluster role binding named ingress-clusterrole-binding
$ kubectl apply -f ingress-clusterrole-binding.yaml

creata ingress controller
$ kubectl apply -f ingress-controller.yaml

create a service account named ingress
$ kubectl apply -f ingress-service.yaml




