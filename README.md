## how to run application

### initial settings

```sh
$ minikube start
$ kuberctl apply -f kubernetes/
$ eval (minikube -p minikube docker-env)
$ helm install kubernetes-sample-web-release web/helm/ -f web/helm/values.yaml -n kubernetes-sample
$ minikube service kubernetes-sample-web-release --url -n kubernetes-sample
```

### upgrade kubernetes config

```sh
$ helm upgrade kubernetes-sample-web-release web/helm/ -f web/helm/values.yaml -n kubernetes-sample
$ minikube service kubernetes-sample-web-release --url -n kubernetes-sample
```
