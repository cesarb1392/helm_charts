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
```shell
helm lint <chart dir>
helm package <char name> -d <chart dir>
helm repo index --url <repo url>
```

### Github pages
- go to Github > repo > settings > pages
- source: deploy from branch
- branch: <target branch>, </root>

### Release updates
```shell
# https://helm.sh/docs/helm/helm_repo_index/
helm repo index . --url <repo url> --merge index.yaml
```


## Contributing

The source code of Helm charts can be found on GitHub: https://github.com/cesarb1392/helm-charts/charts

## License

<!-- Keep full URL links to repo files because this README syncs from main to gh-pages.  -->
[Apache 2.0 License](https://github.com/cesarb1392/helm-charts/blob/main/LICENSE).