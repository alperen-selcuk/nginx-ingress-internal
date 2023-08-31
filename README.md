# nginx-ingress-internal

install nginx ingress controller

```
helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace
```

kubernetes nginx ingress service üzerinde annotation girerek internal IP alması sağlanır.

```cloud.google.com/load-balancer-type: "Internal"```
