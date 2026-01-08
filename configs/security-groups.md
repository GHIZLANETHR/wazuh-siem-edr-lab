# Configuration des Security Groups AWS

## Security Group – Serveur Wazuh
- SSH (22) : autorisé depuis l’IP de l’administrateur
- HTTPS (443) : accès au Dashboard Wazuh
- TCP 1514 : communication agents Wazuh
- TCP 1515 : enrôlement des agents

## Security Group – Client Linux
- SSH (22) : accès administrateur uniquement

## Security Group – Client Windows
- RDP (3389) : accès administrateur uniquement

