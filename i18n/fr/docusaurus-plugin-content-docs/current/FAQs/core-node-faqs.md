---
sidebar_label: FAQ sur les Node Core
hide_table_of_contents: false
sidebar_position: 2
---

# FAQ sur les Node Core

---

### 1. Quels sont les différents types de nodes pris en charge par la Core blockchain?

Sur le réseau Core, un nœud complet Core stocke l'historique complet de la blockchain Core, permettant à quiconque de vérifier l'état de n'importe quel compte. Un nœud complet Core peut prendre plusieurs formes :

- **Nœud complet normal :** pour un usage privé.
- **Nœud complet de validateur :** agit en tant que validateur sur Core, validant les blocs et transactions.
- **Nœud complet RPC :** fournit des services RPC et répond aux requêtes HTTP.

En plus de cela, Core prend également en charge

- **Nœud archive :** stocke toutes les données de la blockchain Core depuis le bloc de genèse.
- **Node de snapshot :** stockent des instantanés pour aider d'autres nodes à synchroniser rapidement le réseau.

### 2. Quels sont les avantages de gérer un nœud Core ?

L'exploitation d'un nœud complet Core offre plusieurs avantages, tels que l'amélioration de la sécurité et de la décentralisation du réseau. Les opérateurs peuvent vérifier les transactions de manière indépendante et ne dépendent pas de tiers. Les validateurs utilisant des nodes complets peuvent participer à la production de blocs et à la validation, ce qui leur permet de potentiellement gagner des récompenses. Les nodes configurés en tant que serveurs RPC fournissent des services précieux au réseau. L'installation nécessite de respecter des spécifications matérielles et de bande passante spécifiques, qui varient en fonction de la fonction du nœud (de base, validateur ou serveur RPC).

### 3. Qu'est-ce qu'un nœud complet Core ? Quelles sont les exigences matérielles/logiciels pour exécuter un nœud complet Core ?

Un nœud complet Core stocke l'historique complet de la blockchain Core, permettant à quiconque de vérifier l'état de n'importe quel compte. Un nœud complet Core peut prendre plusieurs formes :

- **Nœud complet normal :** pour un usage privé.
- **Nœud complet de validateur :** agit en tant que validateur sur Core, validant les blocs et transactions.
- **Nœud complet RPC :** fournit des services RPC et répond aux requêtes HTTP.

**Exigences logicielles :** Actuellement, un nœud complet Core ne peut fonctionner que sur Mac OS X et Linux

**Spécifications matérielles du nœud complet Core Testnet**

| **Requis**       | **Détails**                                                                   |
| ---------------- | ----------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace disque libre                                                    |
| CPU              | 4 cœurs CPU                                                                   |
| RAM              | 8 Go                                                                          |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 5 Mbps |

Pour plus de détails, consultez le [Guide de configuration des nodes complets](../Node/config/full-node.md)

**Spécifications matérielles du nœud complet Core Mainnet**

| **Requis**       | **Details**                                                                   |
| ---------------- | ----------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace disque libre                                                    |
| CPU              | 4 cœurs CPU                                                                   |
| RAM              | 32 Go                                                                         |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 5 Mbps |

Pour plus de détails, consultez le [Guide de configuration des nodes complets](../Node/config/full-node.md)

### 4. Qu'est-ce qu'un nœud RPC Core ? Quelles sont les exigences matérielles/logiciels pour exécuter un nœud RPC Core ?

Les nodes RPC (Remote Procedure Call) sur le réseau Core jouent un rôle essentiel en facilitant l'interaction entre les applications externes et la blockchain Core. Ils servent d'interface à travers laquelle les développeurs et les utilisateurs peuvent interroger et interagir avec la blockchain, ce qui les rend indispensables pour le bon fonctionnement des applications décentralisées (DApps) et d'autres services basés sur la blockchain.

**Exigences logicielles :** Actuellement, un nœud complet Core ne peut fonctionner que sur Mac Os X et Linux.

**Spécifications matérielles du nœud complet Core Testnet**

| **Requis**       | **Details**                                                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace libre sur un disque SSD, gp3, 8k IOPS, 250 Mo/s de débit, latence de lecture \<1 ms. |
| CPU              | 8 cœurs CPU                                                                                                                                  |
| RAM              | 16 Go                                                                                                                                        |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 50 Mbps                                                               |

**Spécifications matérielles du nœud complet Core Mainnet**

| **Requis**       | **Details**                                                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace libre sur un disque SSD, gp3, 8k IOPS, 250 Mo/s de débit, latence de lecture \<1 ms. |
| CPU              | 16 cœurs CPU                                                                                                                                 |
| RAM              | 32 Go                                                                                                                                        |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 50 Mbps                                                               |

Pour plus de détails, consultez le [Guide de configuration des nodes RPC](../Node/config/rpc-node-config.md)

### 5. Qu'est-ce qu'un nœud validateur Core ? Quelles sont les exigences matérielles/logiciels pour exécuter un nœud validateur Core ?

Les validateurs sont essentiels pour sécuriser le réseau en produisant des blocs et en validant les transactions dans le cadre du consensus Satoshi Plus de la blockchain Core.

**Exigences logicielles :** Actuellement, un nœud complet Core ne peut fonctionner que sur Mac Os X et Linux.

**Spécifications matérielles du nœud complet Core Testnet**

| **Requis**       | **Details**                                                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace libre sur un disque SSD, gp3, 8k IOPS, 250 Mo/s de débit, latence de lecture \<1 ms. |
| CPU              | 4 cœurs CPU                                                                                                                                  |
| RAM              | 8 Go                                                                                                                                         |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 10 Mbps                                                               |

**Spécifications matérielles du nœud complet Core Mainnet**

| **Requis**       | **Details**                                                                                                                                  |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Stockage         | 1 To d'espace libre sur un disque SSD, gp3, 8k IOPS, 250 Mo/s de débit, latence de lecture \<1 ms. |
| CPU              | 8 cœurs CPU                                                                                                                                  |
| RAM              | 32 Go                                                                                                                                        |
| Vitesse Internet | Connexion large bande avec une vitesse de chargement/téléchargement de 10 Mbps                                                               |

Pour plus de détails, consultez le [Guide de configuration des nodes validateurs](../Node/config/validator-node-config.md)

### 6. Comment configurer un nœud complet sur la blockchain Core ?

Consultez le guide détaillé [ici](../Node/config/full-node.md) pour savoir comment configurer et exécuter un nœud complet sur le réseau Core.