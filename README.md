# Helmfiles

## Prerequisites

### Helm

```
brew install helm
```

### Helmfile

This allows us to version control things like repo config, chart version, and values in an easy to read YAML format.

```
brew install helmfile
```

### helm diff plugin (recommended)

This allows a uer to generate a diff to check the chart changes before applying.

```
helm plugin install https://github.com/databus23/helm-diff
```

## Executing helmfile

Generating a diff

```
helmfile -f <helmfile> diff
```

Templating a chart (useful when troubleshooting)

```
helmfile -f <helmfile> template
```

Applying changes

```
helmfile -f <helmfile> sync
```


