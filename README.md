## how to run application

```sh
$ minikube start
$ eval (minikube -p minikube docker-env)
$ kubectl apply -f web/deployment.yml
$ kubectl apply -f web/service.yml
$ minikube service kubernetes-sample-service --url
```
