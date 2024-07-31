## Node.js with Heros app with postgres example for docker/kubernetes deployments

Simple nodejs app example with kubernetes deployments and postgres database

<img
    src="https://i.imgur.com/jUeBAiH.png"
    alt="Swagger Page of that application">

### Using docker-compose

* `docker-compose up`

### Using kubernetes with minikube

* Install minikube

* Enable minikube nginx ingress addon
```console
$ minikube addons enable ingress
```

* Apply manifest objects
```console
$ kubectl apply -f kubernetes.yml
```

* Set api.example.internal /etc/hosts to minikube ingress endpoint (see ADDRESS from command kubectl get ingress, usually it's 192.168.49.2)

* Go to swagger page - `api.example.internal/documentation`


### Credits

Project example: [https://github.com/ErickWendel/nodejs-with-postgres-api-example/](https://github.com/ErickWendel/nodejs-with-postgres-api-example/)
