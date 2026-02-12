# Architecture Azure Enterprise - Projet InnovTech ☁️🏛️

## 🎯 Présentation
Conception d'une architecture cloud robuste et sécurisée sur Microsoft Azure pour le projet InnovTech. Ce projet met en œuvre le modèle **Hub-and-Spoke** pour une isolation stricte et une gouvernance centralisée.

## 🚀 Réalisations Techniques
* [cite_start]**Topologie Hub-and-Spoke :** Isolation des environnements Prod et Dev avec un Hub centralisant la sécurité (Bastion, Gateway)[cite: 3492, 3511, 3513].
* [cite_start]**Plan d'Adressage IP :** Subdivision précise d'un espace 172.16.50.0/23 en 4 VNets isolés (/25)[cite: 3493, 3527].
* **Architecture PaaS & Sécurité :**
    * [cite_start]Intégration de services managés : App Service (Premium V3), Azure SQL, Key Vault[cite: 3603, 3605, 3608].
    * [cite_start]Sécurisation via **Private Endpoints (Private Link)** pour supprimer toute exposition publique[cite: 3609, 3614, 3633].
* [cite_start]**Gouvernance & IAM :** Mise en œuvre du RBAC, Azure Policy (Deny Public IP) et accès privilégiés via PIM/MFA[cite: 3585, 3628, 3629, 3639].
* [cite_start]**Administration :** Accès sécurisé aux infrastructures via **Azure Bastion**[cite: 3631, 3700].

## 🏗️ Structure Réseau (VNets)
* [cite_start]**VNet-Hub :** Services d'infrastructure et de sécurité[cite: 3513, 3524].
* [cite_start]**VNet-Prod :** Environnement de production critique[cite: 3513, 3524].
* [cite_start]**VNet-Dev :** Environnement de développement isolé[cite: 3513, 3524].
* [cite_start]**VNet-Libre :** Réserve pour extension future[cite: 3513, 3524].

## 📊 Estimation Budgétaire
[cite_start]Projet optimisé pour un coût mensuel d'environ **1000,00€**, incluant les services PaaS et la redondance[cite: 3680].

## 📂 Structure du dépôt
* `/docs` : Contient le rapport d'architecture complet et le plan d'adressage détaillé.
* `/images` : Schémas d'architecture et diagrammes réseau.
