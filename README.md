# oci-cmp-plugin-example

install manifests
```bash
kubectl apply -f manifests/1.argocd-cm-patch.yaml
kubectl -n argocd patch deployments/argocd-repo-server --patch-file manifests/2.argocd-repo-server-patch.yaml
kubectl apply -f manifests/3.argocd-sample.app.yaml
```

verify

```bash
kubectl get pods -n demo
```
