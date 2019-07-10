# Gate RBAC Helm Chart

This is chart to create minimum RBAC on [Kubernetes](http://kubernetes.io) cluster using [Helm](https://helm.sh) package manager.

## Adding the Repo

You need to add gate-rbac helm packages repository before installing the chart:

```bash
helm repo add gate-rbac https://mufti1.github.io/gate-rbac
```

## Installing the Chart

To install the chart with the release name `gate-rbac`:

```bash
helm install --name gate-rbac gate-rbac
```

## Uninstalling the Chart

To uninstall/delete the `gate-rbac` deployment:

```bash
$ helm delete gate-rbac
```
