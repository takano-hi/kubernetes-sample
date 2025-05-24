## how to run application

```sh
$ minikube start
$ kuberctl apply -f kubernetes/
$ eval (minikube -p minikube docker-env)
$ kubectl apply -f web/kubernetes/
$ minikube service kubernetes-sample-service --url -n kubernetes-sample
```
