[title]: <> (MusiqueDuJour)
[excerpt]: <> (Un site web qui permet de suivre et visualiser vos musiques préférées au fil du temps à travers un calendrier interactif.)
[tags]: <> (web, music, date, french, spotify, svelte, sveltekit, postgres, google, api, deezer, favorite, 2025)

## À propos du projet

**Musique du Jour** est un site web qui permet de suivre et visualiser vos musiques préférées au fil du temps à travers un calendrier interactif.

**En développement depuis :** Début 2025
J'ai eu beaucoup de mal à faire un interface qui tient la route...

**Technologies utilisées:**
- **Frontend:** SvelteKit 5 + TailwindCSS
- **Backend:** Node.js + Drizzle ORM + PostgreSQL
- **Authentification:** Better Auth (multi-provider OAuth)
- **Intégration:** Spotify Web API

---

## Le concept

L'idée est simple : Vous écoutez une musique et elle vous marque vraiment ? Voire vous l'écouter en boucle ? Et bien vous avez juste à ouvrir le site **Musique du Jour** pour :

- **Visualiser** un calendrier musical où chaque jour affiche votre musique préférée
- **Suivre automatiquement** vos musiques favorites sur spotify
- **Marquer manuellement** vos coups de cœur pour des périodes spécifiques
~~- **Découvrir** vos tendances musicales à travers des statistiques~~ (pas encore intégré)

---

## Fonctionnalités

### 📅 Calendrier interactif

- **Visualisation mensuelle/hebdomadaire** : Naviguez à travers vos musiques préférées organisées par date
- **Couvertures d'albums** : Chaque jour affiche la pochette de votre musique du moment
- **Plages de dates** : Une même musique peut s'étendre sur plusieurs jours consécutifs
- **Liens directs** : Cliquez sur une pochette pour écouter directement sur Spotify
- **Interface responsive** : Consultez votre calendrier sur mobile, tablette ou desktop

### 🎧 Suivi automatique Spotify

- **Synchronisation en temps réel** : Un service en arrière-plan synchronise automatiquement vos écoutes
- **Détection des favoris** : Algorithme intelligent qui identifie vos coups de cœur basés sur la répétition d'écoute
~~- **Historique complet** : Gardez une trace de toutes vos écoutes Spotify~~
- **Enrichissement des métadonnées** : Récupération automatique des informations (album, artiste, genres, popularité...)

### 🛠️ Gestion manuelle

- **Ajouter un favori** : Marquez manuellement une chanson comme favorite pour une période spécifique
- **Modifier/supprimer** : Gérez facilement vos favoris existants
- **Recherche Spotify** : Recherchez et ajoutez des chansons directement depuis l'interface
- **Plages personnalisables** : Définissez des dates de début et de fin pour chaque favori (ex: pendant une semaine)

---

## Architecture technique

L'application est construite avec une stack moderne et performante :

- **Base de données PostgreSQL** : Stockage des utilisateurs, chansons, favoris, écoutes et statistiques
- **ORM Drizzle** : Gestion type-safe des requêtes et migrations de base de données
- **Service de synchronisation** : Script Node.js qui tourne en arrière-plan pour récupérer les écoutes Spotify
- **Algorithme de favoris personnalisable** : Système modulaire permettant différentes stratégies de détection automatique



---

## Roadmap

### ✅ Fonctionnalités implémentées

- Calendrier interactif avec vue mensuelle
- Authentification multi-provider (Spotify, GitHub, Google...)
- Synchronisation automatique des écoutes Spotify
- Ajout manuel de favoris
- Algorithme de détection automatique des favoris
- Interface de gestion des favoris

### 📋 À venir

- Statistiques avancées
- Export de données
- Application mobile (déjà possible avec chrome)

---

## Pourquoi Spotify ?

Malgré les nombreux problèmes éthiques liés à Spotify, ce choix s'impose pour une simple raison: Spotify a actuellement le meilleur api disponible aux développeurs, avec les meilleurs intégrations. J'ai pensé à ajouter un support Deezer pendant un moment avant de me rendre compte que l'on ne pouvait plus créer de projet api Deezer, j'attend une officialisation d'une nouvel api avec impatience !