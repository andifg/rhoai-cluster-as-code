# RHOAI Cluster as Code Setup


1. Installl Openshift Gitops Operator


```bash
kustomize build argocd-installation/overlays/<cluster-type> | oc apply -f -
```


2. Setup gitops structure

```bash
kustomize build bootstrap/overlays/<cluster-type>/  | oc apply -f -
```