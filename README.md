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

<br>

## Développeur Frontend (stage de 4 mois)

**[AllForOne Madagascar](https://allforone.mg/fr)** (ESN, Antananarivo) · 15 juin – 15 octobre 2026

**Projet : Madadiaspora**, plateforme communautaire qui relie la diaspora malagasy à Madagascar pour le partage d'informations, l'entraide et le développement socio-économique du pays. J'ai assuré l'intégration du nouveau front-office à partir des maquettes Figma de l'équipe design, connecté à l'API REST de l'équipe backend.

- **Équipe :** 2 développeurs frontend (dont un lead), 1 développeur backend, une équipe design. J'ai réalisé l'intégration seul pendant le stage ; le lead assure la suite.
- **Stack :** Next.js, TypeScript, Tailwind CSS, shadcn/ui, Axios, TanStack Query, Zod, React Hook Form, Git / GitLab.
- **Statut :** livré en environnement de test chez le client, pas encore en production. Le site public affiche encore l'ancienne version, que je n'ai pas développée : il n'y a donc pas de lien direct.
- **Méthode de travail :** réunions techniques, revues de code et tests de validation avec les équipes.

| Mission | Ce que j'ai réalisé | Problèmes résolus |
| ------- | ------------------- | ----------------- |
| **Site vitrine** | Pages intégrées depuis Figma, responsive du mobile au grand écran (non prévu par la maquette), globe 3D interactif (globe.gl), animations (Motion, Magic UI), code organisé en Feature-Sliced Design avec design tokens. | Le globe mettait plus de 5 s à s'afficher sans retour visuel : préchargement de sa texture et loader dédié. Taille et position du globe sur tous les écrans : deux helpers pilotés par breakpoint. |
| **Application web à 7 rubriques** (Actualités, Annuaire, Boîte à projets, Bon à savoir, Diaspor'Album, Événements, Opportunités & Business) | Couche d'accès aux données centralisée (instance Axios, un hook TanStack Query par ressource, durée de cache adaptée à chaque rubrique), layout commun, filtres par pays, secteur et récence, pagination, calendrier mensuel (FullCalendar). | Layout à trois zones sur petit écran : menu replié sous 1280 px, aperçus placés sous le contenu, recherche réduite à une icône sous 640 px. Calendrier : événements limités par jour avec lien « +N », vue en liste sur mobile, chargement par période. Écart entre maquettes et données réelles : cartes à ratio d'image fixe, textes tronqués, images de secours, états de chargement, de vide et d'erreur. |

---

# Projets

## [Tapakila — Plateforme de gestion d'événements](https://tapakila-ui.vercel.app/)

![Tapakila image](assets/img/tapakila.jpg)

**GitHub API :** [tapakila-api](https://github.com/Williest-Andry/tapakila-api) · **GitHub UI :** [tapakila-ui](https://github.com/Williest-Andry/tapakila-ui) · **Démo live :** [tapakila-ui](https://tapakila-ui.vercel.app/)

<!-- Compte de démo : décommente la ligne suivante après avoir créé le compte
**Compte de démo :** e-mail `A_REMPLIR` · mot de passe `A_REMPLIR`
-->

### Description

Plateforme fullstack de réservation de billets d'événements (VIP, Standard, Early Bird) avec gestion des rôles, authentification JWT et interface publique en Next.js 15.

**Contexte :** projet académique de groupe (2025 - [ancien Tapakila](https://github.com/Williest-Andry/Tapakila.git)) que j'ai entièrement refactorisé et étendu en solo : nouvelle architecture, nouvelle stack, nouveau code.

**Mon rôle :** refactorisation complète du backend (Node.js / Express / TypeScript / Prisma / PostgreSQL), conception de l'API REST avec contrat OpenAPI, intégration frontend en TypeScript avec Next.js 15 et Chakra UI v3, mise en place de la couche d'état avec Zustand et TanStack Query.

### Technologies

| Couche    | Stack                                                                      |
| --------- | -------------------------------------------------------------------------- |
| Frontend  | Next.js 15 (App Router), TypeScript, Chakra UI v3, Zustand, TanStack Query |
| Backend   | Node.js, Express, TypeScript, Prisma, PostgreSQL, JWT, OpenAPI 3           |
| Outillage | openapi-fetch, openapi-typescript, Zod                                     |
| Déploiement | Frontend sur Vercel, API en ligne                                        |

### Décisions techniques notables

- **Architecture découplée :** API REST indépendante consommée par un frontend Next.js, chaque couche étant déployable séparément.
- **Typage de bout en bout :** types générés automatiquement depuis le contrat OpenAPI (`openapi-typescript`), zéro type manuel sur les appels API.
- **Authentification robuste :** middleware JWT avec refresh token automatique côté client via intercepteur `openapi-fetch`.
- **Gestion d'état structurée :** Zustand pour l'authentification et le panier de réservation, TanStack Query pour le cache serveur.

---

## MoneyWise — Application mobile de gestion financière personnelle

**Télécharger l'APK :** [Google Drive](https://drive.google.com/file/d/1GG8gQkYXyIyyoBsHDTXU6rX9dc7BlB4X/view?usp=drive_link)  
**Vidéo de démo :** [Voir la démonstration](https://drive.google.com/file/d/1tN60N91cRaIDys7yjPHTHvZVwI2aoBI_/view?usp=drive_link)  
**GitHub :** [public-money-wise](https://github.com/Williest-Andry/public-money-wise.git) _(copie publique du projet collaboratif)_

![MoneyWise image](assets/img/money-wise-resize.png)

### Description

Application mobile React Native de gestion financière personnelle : suivi des dépenses quotidiennes, mensuelles et annuelles, objectifs financiers avec notifications, portefeuilles multi-devises, et une fonctionnalité premium de gestion de budget de projets avec génération de PDF.

Projet réalisé en groupe de 5 dans le cadre d'un examen académique. Le dépôt d'origine est privé.

### Technologies

React Native · Expo · TypeScript · PostgreSQL · Google Auth · Biométrie (empreinte) · Notifications push · Génération PDF

### Mon rôle

- **Module Objectifs (Goals), développé intégralement par moi :** ajout, modification, suppression et affichage paginé des objectifs de dépenses et de revenus, avec filtres par intervalle de dates ; notifications push à chaque échéance, qui redirigent vers l'objectif concerné.
- **Modification de portefeuille :** formulaire d'édition avec validation et mise à jour des statistiques associées.
- **Affichage des projets avec filtres :** écran de liste des projets budget avec filtrage paramétré et navigation vers la vue détaillée.

### Ce qui rend ce projet concret

- APK fonctionnel, téléchargeable et installable directement
- Authentification biométrique (sans mot de passe après la première connexion)
- Notifications push paramétrables par l'utilisateur
- Fonctionnalité premium avec génération et partage de PDF

---

## Autres projets

- **[Gestion de ligues de football](https://github.com/Williest-Andry/football-championship-api.git)** : APIs REST Spring Boot / PostgreSQL / OpenAPI 3 qui agrègent les statistiques des 5 grands championnats européens. Une API locale par championnat et une API centrale qui synchronise et calcule les statistiques globales. J'ai développé seul la partie locale : génération des matchs aller-retour, classements, statistiques avancées, endpoints analytiques filtrés.
- **[Gestion de restaurant](https://github.com/Williest-Andry/sale-point-restaurant.git)** : backend Spring Boot / PostgreSQL / OpenAPI 3 (ingrédients, plats, commandes avec transitions de statut), en deux niveaux : API centrale et API par point de vente, dont j'ai développé la partie point de vente. Architecture Controller / Service / Repository / Mapper et gestion d'erreurs structurée (400, 404, 500).

---

# Compétences

## Frontend

- **Next.js 15** (App Router, Server Components, middleware)
- **React / React Native** (Expo) et **React Admin**
- **TypeScript**
- **TanStack Query v5** (fetching, cache, synchronisation serveur)
- **Axios** (instance configurée, gestion d'erreurs)
- **React Hook Form + Zod** (formulaires et validation)
- **openapi-fetch / openapi-typescript** (client API typé depuis un contrat OpenAPI)
- **Zustand** (état global)
- **Tailwind CSS, shadcn/ui, Chakra UI v3, Nativewind**

## Backend

- **Node.js / Express** (API REST, middlewares, architecture modulaire)
- **Spring Boot** (API REST, architecture en couches)
- **JWT** (access token + refresh token)
- **Prisma** (ORM, migrations)
- **PostgreSQL**

## Conception et outillage

- **Git / GitHub / GitLab** (versioning, branches, pull requests, revues de code)
- **GitHub Actions** (pipelines d'intégration continue)
- **OpenAPI 3** (conception contract-first)
- **Postman** (tests et documentation d'API)
- **Docker** (conteneurisation, déploiement local)
- **Jira, Trello** (suivi de tâches)

## Pratiques

- Architecture découplée frontend / backend
- Typage de bout en bout depuis un contrat OpenAPI
- Authentification JWT avec refresh automatique
- Séparation des responsabilités (Controller / Service / Repository)
- Next.js App Router : Server vs Client Components, Suspense
- Intégration de maquettes Figma responsive
- Gestion systématique des états d'interface (chargement, vide, erreur)
- Pipeline CI/CD avec GitHub Actions

---

# Formation

**Licence informatique** · Haute École d'Informatique, Antananarivo · Octobre 2023 – Novembre 2026
Parcours Écosystème Logiciel (développement web). Soutenance validée en novembre 2026, diplôme en attente de la sortie de promotion.
Cours clés : POO, API REST, Interface web, Sécurité informatique.

# Langues

- Français : B2 (TV5MONDE)
- Anglais : lecture de documentation technique
- Malagasy : langue maternelle
