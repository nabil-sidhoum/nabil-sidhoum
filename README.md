# Nabil SIDHOUM — Tech Lead .NET

> *Je ne me contente pas de livrer des fonctionnalités — je construis des bases sur lesquelles les équipes peuvent travailler avec confiance pendant des années.*

Développeur .NET depuis plus de 10 ans, je me suis spécialisé dans un rôle que peu de gens font vraiment bien : **prendre en charge des plateformes complexes, les restructurer sans tout casser, et les rendre évolutives sur le long terme.**

Mon parcours chez IRBIS Finance en est l'exemple le plus concret. J'ai conçu le MVP initial en tant que consultant, quitté le projet, puis été rappelé deux ans plus tard pour reprendre une base de code qui s'était dégradée : architecture non définie, requêtes SQL sous-performantes, synchronisation CRM qui échouait silencieusement sans que personne ne soit alerté. J'ai refondé l'ensemble en **Clean Architecture modulaire**, réécrit la couche données, mis en place l'observabilité manquante, et migré de **.NET Framework 4.6 vers .NET 8** — le tout en environnement parallèle, sans interruption de service sur une plateforme à **200+ connexions par jour**.

Ce type de chantier — reprendre, stabiliser, moderniser — c'est ce dans quoi je suis le plus à l'aise.

---

## Ce que je fais concrètement

```
├── Conception technique        → Architecture Clean/modulaire, séparation des responsabilités,
│                                 modélisation du domaine métier
├── Développement actif         → API REST, couche domaine, accès aux données (EF Core / SQL Server)
├── Migration & modernisation   → .NET Framework → .NET 8, refonte progressive sans régression
├── Qualité & observabilité     → Revues de code, monitoring, alerting, réduction de dette technique
├── CI/CD                       → Pipelines Azure DevOps, automatisation du déploiement
└── Accompagnement technique    → Encadrement de développeurs, choix d'architecture, montée en compétence
```

---

## Convictions techniques

**Sur l'architecture**
Une bonne architecture ne se voit pas — elle se ressent quand on peut ajouter une fonctionnalité sans avoir peur de casser quelque chose. Je construis des systèmes modulaires où chaque couche a une responsabilité claire, pas des systèmes parfaits sur le papier mais impossibles à maintenir en pratique.

**Sur la dette technique**
Elle est inévitable. Ce qui compte c'est de la rendre visible, de la prioriser honnêtement, et de la résorber progressivement sans bloquer les livraisons. J'ai rarement vu une réécriture complète mieux réussir qu'une refonte incrémentale bien menée.

**Sur les revues de code**
Ce n'est pas un contrôle qualité — c'est un outil de transmission. Une bonne revue de code apprend plus à l'équipe qu'une semaine de formation.

---

## Stack

**Développement**

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)
![.NET 8](https://img.shields.io/badge/.NET_8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Entity Framework Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white)
![Blazor WASM](https://img.shields.io/badge/Blazor_WASM-512BD4?style=flat-square&logo=blazor&logoColor=white)

**Architecture & Pratiques**

![Clean Architecture](https://img.shields.io/badge/Clean_Architecture-1F4E79?style=flat-square)
![DDD](https://img.shields.io/badge/Domain_Driven_Design-1F4E79?style=flat-square)
![TDD](https://img.shields.io/badge/Sensibilité_TDD-1F4E79?style=flat-square)
![Code Review](https://img.shields.io/badge/Code_Review-1F4E79?style=flat-square)

**CI/CD & Outils**

![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azure-devops&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![NuGet](https://img.shields.io/badge/NuGet-004880?style=flat-square&logo=nuget&logoColor=white)
![Dynamics CRM](https://img.shields.io/badge/Dynamics_CRM-0078D4?style=flat-square&logo=microsoft&logoColor=white)

---

## Projets publics

### 🔌 [DynamicsCrmConnector](https://github.com/nabil-sidhoum/DynamicsCrmConnector)

Né d'un besoin réel chez un client : un connecteur propre, injectable et typé pour l'API OData de Microsoft Dynamics CRM, là où les solutions disponibles étaient trop lourdes ou mal maintenues.

- Authentification OAuth2 applicative (ClientId / SecretId), gestion automatique des tokens
- CRUD complet + support FetchXML avec pagination automatique
- Extension typée `Tools.DynamicsCRM.Extensions` pour mapping d'entités fortement typées
- Pipeline NuGet automatisé via GitHub Actions

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)
[![NuGet](https://img.shields.io/nuget/v/Tools.DynamicsCRM.svg?style=flat-square&label=Tools.DynamicsCRM)](https://www.nuget.org/packages/Tools.DynamicsCRM)

---

### ☁️ [OpenstackSwiftConnector](https://github.com/nabil-sidhoum/OpenstackSwiftConnector)

Connecteur HTTP asynchrone pour l'API REST OpenStack Swift, développé pour un contexte de stockage objet OVH. Même philosophie que DynamicsCrmConnector : léger, injectable, sans dépendance superflue.

- Renouvellement automatique des tokens d'authentification OVH OpenStack
- Interface `ISwiftClient` injectable via DI native .NET
- Gestion des conteneurs et upload de fichiers

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white)
[![NuGet](https://img.shields.io/nuget/v/Tools.Swift.Connector.svg?style=flat-square&label=Tools.Swift.Connector)](https://www.nuget.org/packages/Tools.Swift.Connector)

---

### 🗂️ [Portfolio Blazor WebAssembly](https://github.com/nabil-sidhoum/nabil-sidhoum.github.io)

Portfolio en ligne développé en Blazor WebAssembly — parce qu'un Tech Lead .NET qui fait son portfolio en React, c'est un peu dommage. Architecture en composants Razor réutilisables, déploiement automatisé sur GitHub Pages via GitHub Actions.

![Blazor](https://img.shields.io/badge/Blazor_WASM-512BD4?style=flat-square&logo=blazor&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
[![Demo](https://img.shields.io/badge/Demo-nabil--sidhoum.github.io-1F4E79?style=flat-square)](https://nabil-sidhoum.github.io)

---

## Me contacter

[![Portfolio](https://img.shields.io/badge/Portfolio-nabil--sidhoum.github.io-1F4E79?style=flat-square&logo=google-chrome&logoColor=white)](https://nabil-sidhoum.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Nabil_Sidhoum-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nabil-s-32b53ab8)
[![Email](https://img.shields.io/badge/Email-nabil.sidhoum@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:nabil.sidhoum@gmail.com)
