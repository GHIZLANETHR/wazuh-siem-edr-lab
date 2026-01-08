# Installation de l’agent Wazuh – Client Windows

## Environnement
- OS : Windows Server
- Type : Instance EC2

## Méthode d’installation
L’agent Wazuh est installé via **PowerShell**
en tant qu’administrateur, à partir des commandes
générées dans le Dashboard Wazuh.
## Étapes
1. Accéder au Dashboard Wazuh
2. Aller dans **Deploy new agent**
![Agent Windows](../screenshots/windows-agent.png)
3. Sélectionner :
   - Operating system : Windows
4. Copier la commande PowerShell
5. Exécuter la commande dans PowerShell (Admin)
![Commande PowerShell](../screenshots/windows-agent-install.png)
## Vérification
- Le service **Wazuh Agent** est en cours d’exécution
- Les événements Windows Security sont remontés vers le serveur
- ![Commande PowerShell](../screenshots/windows-agent-install2.png)
## Vérification du service
Le service Wazuh Agent est actif.

![Service Wazuh Windows](../screenshots/windows-agent-running.png)
