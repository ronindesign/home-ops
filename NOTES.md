### CRD Installation

When deploying a new app that requires new CRDs, update `bootstrap/helmfile.d/00-crds.yaml` and run:
```
helmfile --file bootstrap/helmfile.d/00-crds.yaml template | kubectl apply --server-side --filename -
```