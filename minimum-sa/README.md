# Gate RBAC Helm Chart

This is chart to create minimum service account on [Kubernetes](http://kubernetes.io) cluster using [Helm](https://helm.sh) package manager.

## Adding the Repo

You need to add minimum-sa helm packages repository before installing the chart:

```bash
helm repo add minimum-sa https://mufti1.github.io/helm-minimum-sa
```

## Installing the Chart

To install the chart with the release name `minimum-sa`:

```bash
helm install --name minimum-sa minimum-sa
```

## Uninstalling the Chart

To uninstall/delete the `minimum-sa` deployment:

```bash
$ helm delete minimum-sa
```
