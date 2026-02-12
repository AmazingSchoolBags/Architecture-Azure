# Architecture Cloud Azure - Projet InnovTech ☁️🔵

## 🎯 Présentation du projet
Conception d'une infrastructure cloud sécurisée sur Microsoft Azure pour la société "InnovTech". Ce projet met en œuvre les meilleures pratiques d'architecture d'entreprise, notamment le modèle **Hub-and-Spoke** et une approche de sécurité **Zero Trust**.

## 🚀 Réalisations Techniques
* **Topologie Réseau :** Mise en place d'une architecture **Hub-and-Spoke** pour centraliser les flux et isoler les environnements.
* **Sécurité & Administration :** * Déploiement d'**Azure Bastion** pour un accès RDP/SSH sécurisé sans IP publiques.
    * Utilisation de **Private Endpoints** pour isoler les services PaaS (App Service, SQL Database) du réseau public.
* **Gouvernance & Identité :** Configuration du RBAC, MFA obligatoire et mise en place de politiques via **Azure Policy**.
* **Postures de Sécurité :** Implémentation du modèle Zero Trust et micro-segmentation réseau via des NSG (Network Security Groups).
* **Monitoring :** Surveillance des performances et alertes via **Azure Monitor**.

## 🏗️ Architecture & Adressage
Le plan d'adressage a été conçu pour éviter tout chevauchement (Overlap) et permettre l'évolutivité :
* **VNet Hub :** Centralisation des services partagés (Bastion, Gateway).
* **VNet Spoke App :** Hébergement de la couche applicative.
* **VNet Spoke Data :** Stockage hautement sécurisé pour les données sensibles.

## 📊 Optimisation des Coûts
Le projet inclut une estimation détaillée des coûts via la calculatrice Azure, optimisant les ressources pour un équilibre performance/prix (Instance B-Series, SQL DTU-based).

## 📁 Documentation
Le rapport technique complet détaillant la feuille de route de migration (Roadmap) et le plan de déploiement (Build Plan) est disponible dans le dossier `/docs`.

## 👥 Auteur
* Mohamed Chaouay Tissir (Formation
