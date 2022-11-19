## Publishing a new the Chart

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/wireguard-bananas)](https://artifacthub.io/packages/search?repo=wireguard-bananas)

### Charts list:
- [wireguard](https://github.com/cesarb1392/helm_charts/tree/main/charts/wireguard)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```console
helm repo add cesarb1392 https://cesarb1392.github.io/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve the latest versions of the packages.

You can then run `helm search repo cesarb1392` to see the charts.

### First time setup
```console
git checkout --orphan gh-pages
git rm -rf .
git commit -m "Initial commit" --allow-empty
git push --set-upstream origin gh-pages

# goto -> GH Settings -> Pages -> check `gp-pages` is selected

git checkout main # index.yaml is managed in gh-pages branch
helm create <chart name>
push helm chart + https://github.com/marketplace/actions/helm-chart-releaser >> .github/workflows/release.yml

Charts.yaml update -> appVersion: "0.1.0"

git push !
```


## Contributing

The source code of Helm charts can be found on GitHub: https://github.com/cesarb1392/helm-charts/charts

## License

<!-- Keep full URL links to repo files because this README syncs from main to gh-pages.  -->
[Apache 2.0 License](https://github.com/cesarb1392/helm-charts/blob/main/LICENSE).