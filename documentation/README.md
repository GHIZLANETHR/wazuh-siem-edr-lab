# Architecture du projet Wazuh SIEM & EDR

## 1. Description générale
Le projet repose sur une infrastructure Cloud déployée sur AWS,
intégrant une solution SIEM et EDR basée sur **Wazuh**.

Un serveur central Wazuh collecte et analyse les événements de sécurité
provenant de deux endpoints :
- Un système Linux
- Un système Windows

Cette architecture permet une supervision centralisée et multi-OS,
similaire à celle utilisée dans un SOC moderne.

## 2. Composants de l’architecture
- **EC2-1 : Serveur Wazuh**
  - OS : Ubuntu 22.04 LTS
  - Mode : All-in-One (Manager, Indexer, Dashboard)

- **EC2-2 : Client Linux**
  - OS : Ubuntu 22.04
  - Agent Wazuh installé

- **EC2-3 : Client Windows**
  - OS : Windows Server
  - Agent Wazuh installé

## 3. Communication et sécurité
Les communications entre les agents et le serveur Wazuh sont contrôlées
par des **Security Groups AWS** avec des règles strictes.
Les ports utilisés sont ceux recommandés par Wazuh (1514, 1515, 443).

## 4. Objectifs de l’architecture
- Centralisation des logs
- Détection des incidents de sécurité
- Analyse SIEM et EDR
- Supervision des endpoints Linux et Windows

