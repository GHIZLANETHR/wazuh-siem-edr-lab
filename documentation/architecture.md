# Architecture générale du laboratoire

## Vue d’ensemble
L’infrastructure repose sur une VPC AWS unique hébergeant
trois instances EC2 communicantes.

![Instances EC2](../screenshots/ec2-instances.png)

Les instances sont :
- Serveur Wazuh (Ubuntu 22.04)
- Client Linux (Ubuntu 22.04)
- Client Windows (Windows Server)

## Groupes de sécurité
Les règles de sécurité sont volontairement restrictives.

![Security Group Wazuh](../screenshots/sg-wazuh.png)
![Security Group Linux](../screenshots/sg-linux.png)
![Security Group Windows](../screenshots/sg-windows.png)

Ces règles garantissent que seules les communications nécessaires
au fonctionnement de Wazuh sont autorisées.

