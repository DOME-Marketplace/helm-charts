# HELM CHARTS

A helm repository for DOME.

## Usage

 1. Clone this repository.
 2. Create a new branch.
 3. Create a new folder.
 4. Package your charts. This step will generate a `.tgz` file.

```bash
helm package <path to your charts>
```

 5. Move the `.tgz` files to your folder.
 6. Create the `index.yaml` file.

```bash
helm repo index . --url https://dome-marketplace.github.io/helm-charts/<your folder name>
```
> 💡 Add `--merge index.yaml` if you want to update the charts.

 7. Update the `repositories.yaml` with your chart name, URL and related repositories.
 8. Create a pull request to the `gh-pages` branch.