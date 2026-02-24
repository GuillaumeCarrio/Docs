# Creation du contenu de l'EKS depuis la console

## Créer le cluster

```bat
export EKS_CLUSTER_NAME=eks-workshop

curl -fsSL https://raw.githubusercontent.com/aws-samples/eks-workshop-v2/stable/cluster/eksctl/cluster.yaml | \
envsubst | eksctl create cluster -f -
```

## Créer l'environnement

```bat
prepare-environment introduction/getting-started
```

```bat
prepare-environment
```
