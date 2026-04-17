# Ajout d'un agent sur Wazuh

## Linux

Pour ajouter l'agent sous Linux, on va aller dans le AGENT SUMMARY en haut a gauche et cliquer sur "Active (0)"

![Wazuh Agent Actifs](../Pictures/ActiveAgentWazuh.png)

On va clicker sur "Deploy new agent"

![Wazuh Agent New](../Pictures/DeployNewAgentWazuh.png)

1. Cocher DEB amd64.
2. Mettre l'IP privée de l'EC2 Wazuh.
3. Mettre le nom de l'EC2 qu'on souhaite lier.
4. Copier la commande donnée.

Exécuter cette commande dans la console de l'instance EC2 de la VM qu'on souhaite monitorer.

Entrer les commandes suivantes :

```bat
sudo systemctl daemon-reload
```

```bat
sudo systemctl enable wazuh-agent
```

```bat
sudo systemctl start wazuh-agent
```

Retourner à la liste dess Agents et attendre.
Si vous n'avez pas fait d'erreur, tout devrait être bon.

## Windows

Pour ajouter l'agent sous Windows, on va aller dans le AGENT SUMMARY en haut a gauche et cliquer sur "Active (0)"

![Wazuh Agent Actifs](../Pictures/ActiveAgentWazuh.png)

On va clicker sur "Deploy new agent"

![Wazuh Agent New](../Pictures/DeployNewAgentWazuh.png)

1. Cocher MSI 32/64 bits.
2. Mettre l'IP privée de l'EC2 Wazuh.
3. Mettre le nom de l'EC2 qu'on souhaite lier.
4. Copier la commande donnée.

Exécuter cette commande dans un powershell sur la VM qu'on souhaite monitorer.

Entrer la commande suivante :

```bat
NET START Wazuh
```

Retourner à la liste dess Agents et attendre.
Si vous n'avez pas fait d'erreur, tout devrait être bon.
