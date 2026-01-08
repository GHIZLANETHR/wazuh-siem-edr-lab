# Installation du serveur Wazuh

## Environnement
- Cloud : AWS Learner Lab
- Instance : EC2
- OS : Ubuntu 22.04 LTS

## Mode d’installation
Le serveur Wazuh est installé en mode **All-in-One**,
incluant :
- wazuh-manager
- wazuh-indexer
- wazuh-dashboard

## Commande d’installation
L’installation est effectuée via le script officiel Wazuh :

```bash
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh
sudo bash wazuh-install.sh -a
<img width="945" height="561" alt="image" src="https://github.com/user-attachments/assets/f4fc7585-bc26-4fc5-b3cf-adcbbfb7444a" />

