```bash
argocd app create nginx \
 --repo https://github.com/akashkaturi/ArgocdCloud.git \
 --path charts/app_chart \
 --sync-policy auto \
 --dest-namespace argocd \
 --dest-server https://kubernetes.default.svc
```
