
---

## 📄 `installation/linux-agent.md`

```markdown
# Installation de l’agent Wazuh – Client Linux

## Environnement
- OS : Ubuntu 22.04
- Type : Instance EC2

## Méthode d’installation
L’agent Wazuh est déployé directement depuis le **Dashboard Wazuh**
en utilisant l’assistant **Deploy new agent**.

## Étapes
1. Accéder au Dashboard Wazuh
2. Aller dans la section **Agents**
3. Cliquer sur **Deploy new agent**
4. Sélectionner :
   - Operating system : Linux
   - Architecture : x86_64
   - IP privée du serveur Wazuh
5. Copier les commandes générées
6. Exécuter les commandes sur le client Linux

## Vérification
Après installation et démarrage de l’agent :
- L’agent apparaît avec l’état **Active**
- Les événements sont visibles dans le SIEM
