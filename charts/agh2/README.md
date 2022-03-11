# AGH2-helm

## Usage

To install the latest version of this chart, download the Argushack helm repository and copy `values.yaml` as new file then fill the Database information & API Token.

After finished above, run `helm install` with new `values.yaml`:

``` bash
helm install agh . -f deployment-values.yaml
```

To install with namespace created:

``` bash
helm install agh . -f deployment-values.yaml --namespace agh --create-namespace
```

To upgrade AGH, run `helm upgrade`:

``` bash
# default namespace
helm upgrade agh . -f deployment-values.yaml -f upgrade.yaml

# specify namespace
helm upgrade agh . -f deployment-values.yaml -f upgrade.yaml --namespace agh
```
