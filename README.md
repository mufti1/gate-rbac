# Minimum Service Account Helm Packages

Maintains the Helm packages of minimum-sa.

## Using the Packages

Add packages repo in Helm:

```bash
helm repo add minimum-sa https://mufti1.github.io/helm-minimum-sa
```

Install `minimum-sa` package with release name minimum-sa:

```bash
helm install --name minimum-sa minimum-sa/minimum-sa
```

Adding New Package

1. Clone this repo.
2. Go to `minimum-sa` folder.
3. Update the chart and app version in `Chart.yaml`.
4. Execute `$ helm package .`, this will create file `minimum-sa-x.y.z.tgz`, where x, y, z are the new version number that automatically generated from step 3.
5. Move `minimum-sa-x.y.z.tgz` to the top of folder in this repo.
6. Execute `$ helm repo index . --url https://mufti1.github.io/helm-minimum-sa`, this will update the `index.yaml` file.
7. Commit and push changes.
