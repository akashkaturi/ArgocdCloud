```bash
argocd app create nginx \
 --repo https://github.com/akashkaturi/ArgocdCloud.git \
 --path charts/app-chart \
 --sync-policy auto \
 --dest-namespace argocd \
 --dest-server https://kubernetes.default.svc
```

```bash

echo -n '{"auths":{"https://index.docker.io/v1/":{"username":"akashkaturi","password":"password","email":"akashkaturi77@gmail.com","auth":"YWthc2hrYXR1cmk6YWthc2hsbXNkOTEwMTE="}}}' | base64
```
