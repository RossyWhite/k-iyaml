# k-iyaml

A plugin to view yaml formatted kubernetes resource with an interactive selector.
  
## Requirements

- [fzf](https://github.com/junegunn/fzf)
- [yh](https://github.com/andreazorzetto/yh)

## Installation

```bash
export INSTALL=<yourpath> # anywhere inside $PATH
curl https://raw.githubusercontent.com/RossyWhite/k-iyaml/master/kubectl-iyaml -o $INSTALL/kubectl-iyaml
```

## Usage

```bash
$ kubectl iyaml --help

Usage: kubectl iyaml [OPTIONS...] <resource> <query>
OPTIONS:
  -h, --help               Show help for 'kubectl iyaml'
  -n, --namespace string   The name of namespace to use
  --context string         The name of kubeconfig context to use
Examples: 
  kubectl iyaml deployment -n kube-system --context my-cluster
  kubectl iyaml service api -n default
```
