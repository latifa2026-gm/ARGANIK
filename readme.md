# 🌿 Roadmap du Projet : Site Vitrine Arganik

> **Client :** Coopérative féminine Arganik (Souss-Massa)
>
> **Agence :** Atlas Digital
>
> **Type de projet :** Site vitrine 5 pages, Responsive & Accessible (HTML5 / CSS3 Flexbox)
>
> **Période du projet :** 12/10/2026 au 16/10/2026 (5 jours)

## 🎯 Scope & Objectifs Technologiques

* **Architecture :** Multi-pages HTML5 Sémantique (5 pages distinctes).

* **Stylisation :** CSS3 Moderne & Flexbox (Optionnel : CSS Grid, Tailwind CSS).

* **Approche Design :** Mobile-First (aucun défilement horizontal de 320px à 1440px+).

* **Accessibilité (a11y) :** Navigation au clavier, attributs `alt` pertinents sur les images, contrastes conformes WCAG, structuration unique de `<h1>`.

* **Versioning & Git Flow :** Stratégie de branches strictes avec Pull Requests (PR) obligatoires pour chaque fonctionnalité.

* **Formulaire :** Validations natives HTML5 (`email`, `tel`, `required`).

## 📅 Timeline & Jalons (Milestones)

```
[Jour 1 - 12/10] ──> [Jour 2 - 13/10] ──> [Jour 3 - 14/10] ──> [Jour 4 - 15/10] ──> [Jour 5 - 16/10]
  Cadrage, Git &      Header/Footer &       Développement         Finalisation,          Recette, Bonus &
  Planification       Premier Livrable      des Pages             Audits & W3C           Livrable Final
```

## 📑 Répartition des Rôles & Tâches (Équipe de 5)

| Rôle / Membre | Responsabilité Principale (Page) | Élément Commun / Tâche Transversale | 
| ----- | ----- | ----- | 
| **GOUMIH Latifa** | 🏠 `index.html` (Accueil) |cette page avec sa style css et responsive de cette page .
| **EL GADIRI Aamr** | 🛍️ `pages/produits.html` (Nos Produits) |  cette page avec sa style css et responsive de cette page. 
| **QADDOURA Mohamed** | 🧴 `pages/produit_page.html` (Fiche Produit) | Composants de cartes produits & Badges  et responsive de cette page.| 
| **AIT AHMED Samiya** | 🌳 `pages/tracability2.html` (Traçabilité) |cette page avec sa style et responsive de cette page | Footer commun & Newsletter (`footer.css`) | cette page avec sa style css | 
| **OUCHTAHRICHT Hamza** | ✉️ `pages/contact.html` (Contact & Commande)  |cette page avec sa style et responsive de cette page| Header dynamique & Navigation mobile (`header.css`) | 

## 🗓️ Feuille de Route Détaillée (Jour par Jour)

### 📌 Jour 1 — Cadrage, Architecture & Git Flow (12/10/2026)

* **09:30 - Lancement du brief & Analyse de la Maquette Figma.**

* **Configuration de l'espace de travail :**

  * Création du projet Trello / GitHub Projects.

  * Découpage des User Stories en tâches fines et assignation.

  * Initialisation du Repository Git local & distant.

  * Configuration de la branche `develop`.

* **Arborescence du Projet :**

  ```text
  ARGANIK/
  ├── css/
  │   ├── accueil.css
  │   ├── produits.css
  │   ├── produit_page.css
  │   ├── tracability2.css
  │   ├── contact.css
  │   ├── footer.css
  │   └── header.css
  ├── pages/
  │   ├── produits.html
  │   ├── produit_page.html
  │   ├── tracability2.html
  │   └── contact.html
  ├── assets/
  │   ├── img/
  │   └── icons/
  ├── index.html
  └── ROADMAP.md
  ```

* **Git Flow Setup :**

  * Protection de la branche `main`.

  * Normalisation des commits : `feat:`, `fix:`.

### 📌 Jour 2 — Header/Footer, Squelettes & 📦 Livrable 1 (13/10/2026)

* **Développement des Composants Communs :**

  * Intégration du Header dans `css/header.css` (Bandeau d'annonce, Logo, Nav active, Panier avec badge, Avatar, Menu burger CSS/HTML).

  * Intégration du Footer dans `css/footer.css` (Horaires, Liens, Réseaux sociaux, Newsletter, 4 Labels, Copyright).

* **Création des squelettes HTML5** sémantiques pour la page principale (`index.html`) et les pages secondaires (`pages/produits.html`, `pages/produit_page.html`, `pages/tracability2.html`, `pages/contact.html`).

* **Intégration du Design System CSS** (Palette de couleurs du Souss, typographies, styles de boutons réutilisables).

#### 🚨 LIVRABLE 1 (Avant 23:59)

1. Lien vers le tableau Trello / GitHub Projects (toutes les User Stories découpées et assignées).

2. Lien du Repository GitHub contenant :

   * Structure complète des fichiers.

   * Header (`css/header.css`) et Footer (`css/footer.css`) intégrés.

   * Branches `main` et `develop`.

   * `README.md` initialisé.

### 📌 Jour 3 — Développement Core des 5 Pages (14/10/2026)

Chaque développeur travaille isolément sur sa branche `feat/<nom-feature>` :

* **🏠 Page Accueil (`faet/accueil`) :**
  * Fichiers : `index.html` & `css/accueil.css`.
  * Hero section avec image de fond, CTAs et 3 engagements.
  * Section 4 chiffres clés & 4 cartes produits phares.
  * Section Impact (Citation présidente & engagements).
  * « De l'arbre au flacon », bandeau d'origine et témoignages.

* **🛍️ Page Nos Produits (`feat/produits`) :**
  * Fichiers : `pages/produits.html` & `css/produits.css`.
  * En-tête avec Fil d'Ariane & Encadré « 100% Bio & Équitable ».
  * Barre de 5 catégories + Panneau de filtres.
  * Grille responsive de 8 cartes produits avec boutons.
  * Pagination & Bandeau réassurance vert.

* **🧴 Page Fiche Produit (`feat/produit_page.html`) :**
  * Fichiers : `pages/produit_page.html` & `css/produit_page.css`.
  * Galerie (Grande image + 4 miniatures).
  * Bloc d'achat (Badges, prix, stock, choix contenances, quantité, boutons d'action).
  * Accordéon CSS « Passeport Terroir » & « Secrets de Fabrication » en 4 étapes.
  * Section 3 avis clients + 4 produits similaires.

* **🌳 Page Traçabilité (`feat/tracability`) :**
  * Fichiers : `pages/tracability2.html` & `css/tracability2.css`.
  * Bloc « Vérifier l'authenticité d'un lot ».
  * 6 étapes de fabrication alternées en desktop / empilées en mobile.
  * Cartes des 3 coopératrices & 4 certifications.

* **✉️ Page Contact & Commande (`feat/contact`) :**
  * Fichiers : `pages/contact.html` & `css/contact.css`.
  * Formulaire de contact complet avec attributs de validation HTML5.
  * Coordonnées atelier, carte d'accès et modalities d'expédition.
  * FAQ à 4 questions & Callout téléphonique.

### 📌 Jour 4 — Mobile-First, Accessibilité & Validations (15/10/2026)

* **Revue Responsive (Mobile-First) :**

  * Tests sur Viewports :  768px, 1024px.

* **Git Flow & Merges :**

  * Revue des PRs individuelles vers `develop`.

  * Résolution des conflits et merge final de `dev` vers `main`.(nous trouvons un probleme dans ce merge !)

### 📌 Jour 5 — Bonus, Déploiement, Support & 📦 Livrable 2 (16/10/2026)

* **Déploiement en ligne :**

  * Publication du site via GitHub Pages.  https://latifa2026-gm.github.io/ARGANIK/

#### 🚨 LIVRABLE 2 (Avant 23:59)

1. Repository GitHub mis à jour avec historique Git Flow propre.

2. `README.md` complet (Présentation,tableau de répartition, lien du site).

3. Lien du site déployé en ligne.

5. Lien du projet Trello .

## 🧪 Grille de Contrôle / Checklist Qualité

* \[ \] **Sémantique HTML5 :** `header`, `nav`, `main`, `section`, `article`, `footer` correctement employés.

* \[ \] **Titres :** Exactement un seul `<h1>` par page.

* \[ \] **Style CSS :** Layouts bâtis avec Flexbox, pas de styles inline. Fichiers CSS associés correctement reliés (`css/header.css`, `css/footer.css`, etc.).

* \[ \] **Accessibilité :** Images avec `alt` informatifs, formulaires avec `<label>` liés via `for`/`id`.

* \[ \] **Formulaire :** Validations `required`, `type="email"`, `type="tel"`.

* \[ \] **Git :** Commits réguliers (`feat:`, `fix:`), branches de features isolées, aucune modification directe sur `main`.
