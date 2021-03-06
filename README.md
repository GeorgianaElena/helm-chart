[![CI Status](https://github.com/dask/helm-chart/workflows/CI/badge.svg)](https://github.com/dask/helm-chart/actions)
[![Dask Chart version](https://img.shields.io/badge/dynamic/yaml?url=https://helm.dask.org/index.yaml&label=chart&query=$.entries.dask[:1].version&color=277A9F)](https://helm.dask.org/)
[![DaskHub Chart version](https://img.shields.io/badge/dynamic/yaml?url=https://helm.dask.org/index.yaml&label=chart&query=$.entries.daskhub[:1].version&color=277A9F)](https://helm.dask.org/)
[![Dask version](https://img.shields.io/badge/dynamic/yaml?url=https://helm.dask.org/index.yaml&label=Dask&query=$.entries.dask[:1].appVersion&color=D67548)](https://helm.dask.org/)



Dask Helm Charts
================

This repository contains Dask's two helm charts.

- [dask](./dask/README.md): Install Dask on Kubernetes for a single user with Jupyter and dask-kubernetes.
- [daskhub](./daskhub/README.md): Install Dask on Kubernetes for multiple users with JupyterHub and Dask Gateway.

## Single-user Quickstart

Users deploying Dask for a single user should use the `dask/dask` helm chart.

```
helm repo add dask https://helm.dask.org/
helm repo update
helm install --name my-release dask/dask
```

See [dask](./dask/README.md) for more.

## Multi-user Quickstart

Users deploying Dask for multiple users should use the `dask/daskhub` helm chart.

```
helm repo add dask https://helm.dask.org/
helm repo update
helm install --name my-release dask/daskhub
```

See [daskhub](./daskhub/README.md) for more.
