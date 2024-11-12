
# Prereq

- Install Helm
- Set admin password:

```shell
apt-get update
apt-get install apache2-utils
```

# Deploy

```shell
helm upgrade -i --atomic --create-namespace -n argocd -f "/c/projects/Personal/argo-cd/values.yaml" argocd argo/argo-cd
```

```shell
helm upgrade -i --atomic --create-namespace -n argocd nginx ingress-nginx/ingress-nginx
```
