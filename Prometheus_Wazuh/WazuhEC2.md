# Create EC2 Wazuh

## Paramètrage de l'instance

On crée une Instance en t3.large avec 30Go et la vockey.

Il faut penser à ajouter les 2 security-groups (All et Wazuh).

### All

Le security group All contient 2 entry :

TCP personnalisé depuis le 0.0.0.0/0 avec le port 22

Tout sur tout depuis lui-même

### Wazuh

TCP personnalisé depuis le 0.0.0.0/0 avec le port 80

TCP personnalisé depuis le 0.0.0.0/0 avec le port 22

TCP personnalisé depuis le 0.0.0.0/0 avec le port 443
