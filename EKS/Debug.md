# Debug

Veuillez trouver ci-après les erreurs les plus fréquentes et la manière de les corriger en autonomie

## En cas d'erreur de suppression due au load balancer comme celle qui suit

![Load Balancer Error](../Pictures/ErrorLoadBalancer.png)

Se rendre sur les LoadBalancer de l'EC2

![EC2 Load Balancer](../Pictures/EC2LoadBalancer.png)

Et le supprimer à la main

![EC2 Load Balancer Suppression](../Pictures/DeleteLoadBalancer.png)

## Il se peut que cela soit insuffisant. On peut le voir avec une erreur à la recréation de la ressource du cluster

![Erreur à la création de ressource](../Pictures/ErrorCreateCluster.png)

Dans ce cas, il va falloir vérifier les traces résiduelles liées à notre VPC ide comme les security group et les supprimer à la main le cas échéant

![Security Group liés au VPC](../Pictures/VPCSecurityGroup.png)

![Suppression du groupe de sécurité](../Pictures/DeleteSecurityGroup.png)
