# minimal-reproduction-template

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).


## Current behavior

HelmChartInflationGenerators defined in Kustomize are not being picked up by Renovate.
The file itself is being picked up because of the customized Renovate config, but only one package is detected.
```
DEBUG: Matched 2 file(s) for manager kustomize: app1/argocd-chart.yaml, app1/kustomization.yaml
DEBUG: manager extract durations (ms)
{
  "managers": {
    "kustomize": 11
  }
}

DEBUG: Found kustomize package files
DEBUG: Found 1 package file(s)
```

## Expected behavior

HelmChartInflationGenerator are detected and Renovate should be able to update the HelmChartInflationGenerator.

## Link to the Renovate issue or Discussion

Lnk to the Renovate Discussion [here](https://github.com/renovatebot/renovate/discussions/32519).
