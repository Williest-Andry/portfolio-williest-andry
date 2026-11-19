# Développeur Fullstack

**Williest ANDRY NY AINA**, Développeur Fullstack à Antananarivo, Madagascar. **Disponible immédiatement.**

**Licence informatique** à la Haute École d'Informatique (parcours Écosystème Logiciel : **développement web** et cloud). Soutenance validée, diplôme en attente de délivrance.

**Mon approche** : concevoir des architectures simples et propres, écrire du code maintenable et livrer des interfaces utilisables. Je maîtrise aussi bien la construction d'une API REST sécurisée que l'intégration côté frontend avec des outils modernes.

**[Télécharger mon CV (PDF)](https://drive.google.com/file/d/1xsc87H3w37evb_sMPgTFVEOgg4GPgiHN/view?usp=sharing)**

- E-mail : [williestnyainaandry@gmail.com](mailto:williestnyainaandry@gmail.com)
- Téléphone : [+261 32 87 774 77](tel:+261328777477)
- LinkedIn : [linkedin.com/in/williest-andry](https://www.linkedin.com/in/williest-andry)
- GitHub : [github.com/Williest-Andry](https://github.com/Williest-Andry)


<br>

# Expérience professionnelle

## Développeur Frontend (stage), [AllForOne](https://allforone.mg/fr) (ESN, Antananarivo)
*15 juin – 15 octobre 2026*

Projet : **Madadiaspora**, plateforme qui relie la diaspora malagasy à Madagascar pour le développement socio-économique du pays. J'ai assuré **l'intégration du nouveau front-office (site vitrine et application web à 7 rubriques)** à partir des maquettes Figma de l'équipe design et **connecté à l'API REST** de l'équipe backend.

- **Site vitrine :** globe 3D interactif (globe.gl), responsive du mobile au grand écran, chargement du globe fluidifié (préchargement de la texture, loader). **5 pages intégrées.**
- **Application web à 7 rubriques :** couche d'accès aux données centralisée (Axios, TanStack Query avec cache adapté), filtres, pagination, calendrier d'événements, interface robuste face aux données réelles (états de chargement, vide, erreur).
- **Stack :** Next.js, TypeScript, Tailwind CSS, shadcn/ui, Axios, TanStack Query, Zod, React Hook Form, GitLab.
- **Statut :** livré en test chez le client, pas encore en production.

<br>

# Projets

## [Tapakila - Plateforme de gestion d'événements](https://tapakila-ui.vercel.app/)

![Tapakila image](assets/img/tapakila.jpg)

**GitHub API :** [tapakila-api](https://github.com/Williest-Andry/tapakila-api) · **GitHub UI :** [tapakila-ui](https://github.com/Williest-Andry/tapakila-ui) · **Démo live :** [tapakila-ui](https://tapakila-ui.vercel.app/)

<!-- 
**Compte de démo :** e-mail `A_REMPLIR` · mot de passe `A_REMPLIR`
-->

### Description

Plateforme de réservation de billets d'événements (VIP, Standard, Early Bird) avec gestion des rôles, authentification JWT et interface publique en Next.js 15.

**Contexte :** projet académique de groupe (2025 - [ancien Tapakila](https://github.com/Williest-Andry/Tapakila.git)) que j'ai entièrement refactorisé et étendu en solo : nouvelle architecture, nouvelle stack, nouveau code.

**Mon rôle :** **refactorisation complète du backend** (Node.js / Express / TypeScript / Prisma / PostgreSQL), **conception de l'API REST avec contrat OpenAPI**, **intégration frontend** en TypeScript avec Next.js 15 et Chakra UI v3, mise en place de la couche d'état avec Zustand et TanStack Query.

### Technologies

| Couche    | Stack                                                                      |
| --------- | -------------------------------------------------------------------------- |
| Frontend  | Next.js 15 (App Router), TypeScript, Chakra UI v3, Zustand, TanStack Query |
| Backend   | Node.js, Express, TypeScript, Prisma, PostgreSQL, JWT, OpenAPI 3           |
| Outillage | openapi-fetch, openapi-typescript, Zod                                         |

### Décisions techniques notables

- **Architecture découplée :** API REST indépendante consommée par un frontend Next.js, chaque couche étant déployable séparément.
- **Typage de bout en bout :** types générés automatiquement depuis le contrat OpenAPI (`openapi-typescript`), zéro type manuel sur les appels API.
- **Authentification robuste :** middleware JWT avec refresh token automatique côté client via intercepteur `openapi-fetch`.

<br>

---

## MoneyWise - Application mobile de gestion financière personnelle

**Télécharger l'APK :** [Google Drive](https://drive.google.com/file/d/1GG8gQkYXyIyyoBsHDTXU6rX9dc7BlB4X/view?usp=drive_link)  
**Vidéo de démo :** [Voir la démonstration](https://drive.google.com/file/d/1tN60N91cRaIDys7yjPHTHvZVwI2aoBI_/view?usp=drive_link)  
**GitHub :** [public-money-wise](https://github.com/Williest-Andry/public-money-wise.git) _(copie publique du projet collaboratif)_

![MoneyWise image](assets/img/money-wise-resize.png)

### Description

Application mobile de gestion financière personnelle : suivi des dépenses quotidiennes, mensuelles et annuelles, objectifs financiers avec notifications, portefeuilles multi-devises, et une fonctionnalité premium de gestion de budget de projets avec génération de PDF.

Projet réalisé en groupe de 5 dans le cadre d'un examen académique. Le dépôt d'origine est privé.

### Technologies

React Native · Expo · TypeScript · PostgreSQL · Google Auth · Biométrie (Fingerprint) · Notifications push · Génération PDF

### Mon rôle

- **Module Objectifs (Goals), développé intégralement par moi :** ajout, modification, suppression et affichage paginé des objectifs de dépenses et de revenus, avec filtres par intervalle de dates, notifications push à chaque échéance, qui redirigent vers l'objectif concerné.
- **Modification de portefeuille :** formulaire d'édition avec validation et mise à jour des statistiques associées.
- **Affichage des projets avec filtres :** écran de liste des projets budget avec filtrage paramétré et navigation vers la vue détaillée.

### Ce qui rend ce projet concret

- APK fonctionnel, téléchargeable et installable directement
- Notifications push paramétrables par l'utilisateur
- Fonctionnalité premium avec génération et partage de PDF

<br>

---

## Autres projets

- **[Gestion de ligues de football](https://github.com/Williest-Andry/football-championship-api.git)** : APIs REST Spring Boot / PostgreSQL / OpenAPI 3 qui agrègent les statistiques des 5 grands championnats européens. Une API locale par championnat et une API centrale qui synchronise et calcule les statistiques globales. J'ai développé seul la partie locale : génération des matchs aller-retour, classements, statistiques avancées, endpoints analytiques filtrés.
- **[Gestion de restaurant](https://github.com/Williest-Andry/sale-point-restaurant.git)** : backend Spring Boot / PostgreSQL / OpenAPI 3 (ingrédients, plats, commandes avec transitions de statut), en deux niveaux : API centrale et API par point de vente, dont j'ai développé la partie point de vente. Architecture Controller / Service / Repository / Mapper et gestion d'erreurs structurée (400, 404, 500).

<br>

# Compétences

## Frontend

JavaScript, TypeScript, React, Next.js, React Native, React Admin, TanStack Query, Axios, React Hook Form, Zod, Zustand, Tailwind CSS, shadcn/ui, Chakra UI

## Backend

Node.js, Express.js, Spring Boot, JWT, Prisma, PostgreSQL

## Outils

Git, GitHub, GitLab, GitHub Actions, OpenAPI 3, Postman, Docker, Jira, Trello

## Notions

- Next.js App Router
- Typage de bout en bout depuis un contrat OpenAPI
- Architecture découplée frontend / backend
- Intégration de maquettes Figma responsive
- Gestion systématique des états d'interface (chargement, vide, erreur)
- Authentification JWT avec refresh automatique
- Séparation des responsabilités (Controller / Service / Repository)
- Pipeline CI/CD avec GitHub Actions

<br>

# Formation

**Licence informatique** - Haute École d'Informatique, Antananarivo, Octobre 2023 – Novembre 2026

Soutenance validée, diplôme en attente de délivrance.

Parcours **Écosystèmes Logiciels (développement web)**. 
Cours clés : POO, API REST, Interface web, Sécurité informatique.

<br>

# Langues

- Français : B2 (TV5MONDE)
- Anglais : lecture de documentation technique
- Malagasy : langue maternelle
