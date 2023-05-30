# MetalLB

## Install

```bash
helm pull \
  oci://registry-1.docker.io/bitnamicharts/metallb

helm upgrade --install \
  metallb \
  -n metallb \
  --create-namespace \
  oci://registry-1.docker.io/bitnamicharts/metallb
```

```yaml
config: |
    address-pools:
    - addresses:
      - 10.57.1.128/29
      name: default
      protocol: layer2
```
