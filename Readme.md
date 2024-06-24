argocd app create helloworld \
 --repo https://github.com/akashkaturi/argo-cd-helm-deployments.git \
 --path charts/helloworld \
 --sync-policy auto \
 --dest-namespace argocd \
 --dest-server https://kubernetes.default.svc
