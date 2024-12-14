# ExamenFlutter
# Documentation du Développement de l'Application DMC Computer

## Introduction
L'application DMC Computer est une plateforme de commerce électronique développée en Flutter, permettant aux utilisateurs de naviguer dans les produits, de filtrer par catégorie et de gérer leurs favoris.

## Étapes de Développement

### 1. Configuration de l'Environnement
- *Installation de Flutter* : Assurez-vous d'avoir Flutter installé sur votre machine.
- *Création du Projet* : Utilisez la commande flutter create dmc_computer pour créer un nouveau projet Flutter.

### 2. Dépendances
Ajoutez les dépendances nécessaires dans le fichier pubspec.yaml :
yaml
dependencies:
  flutter:
    sdk: flutter
  image_picker: ^0.8.4+4
  http: ^0.13.4


### 3. Structure de l'Application
- *Main.dart* : Le fichier principal contenant la logique de l'application.
- *Widgets* : Création de widgets pour la mise en page de l'application, y compris la barre d'application, le tiroir de navigation, et la grille de produits.

### 4. Récupération des Données
- *Produits* : Utilisation de l'API WooCommerce pour récupérer les produits via la méthode http.get.
- *Catégories* : Récupération des catégories de produits pour permettre le filtrage.

### 5. Affichage des Données
- *Grille de Produits* : Utilisation de GridView.builder pour afficher les produits récupérés.
- *Filtrage par Catégorie* : Implémentation d'une méthode pour récupérer et afficher les produits selon la catégorie sélectionnée.

### 6. Gestion des Favoris
- Ajout d'une fonctionnalité pour marquer les produits comme favoris avec un IconButton.

## Fonctionnalités Ajoutées
- *Affichage des Produits* : Les utilisateurs peuvent voir les produits disponibles avec leur nom et prix.
- *Filtrage par Catégorie* : Les utilisateurs peuvent filtrer les produits en fonction de la catégorie sélectionnée, ce qui améliore l'expérience utilisateur.
- *Gestion des Favoris* : Les utilisateurs peuvent ajouter ou retirer des produits de leur liste de favoris.

## Techniques Utilisées
- *Flutter* : Framework pour le développement d'applications multiplateformes.
- *HTTP Requests* : Utilisation du package http pour effectuer des requêtes API.
- *JSON Parsing* : Traitement des données JSON pour afficher les produits et catégories.
- *State Management* : Utilisation de setState pour gérer l'état de l'application lors de la récupération des données.

## Conclusion
Ce projet démontre l'utilisation de Flutter pour créer une application de commerce électronique simple mais fonctionnelle, intégrant des fonctionnalités modernes comme le filtrage dynamique et la gestion des favoris.

---

### Présentation Illustrant les Fonctionnalités

1. *Page d'Accueil* :
   - Présentation de la liste des catégories en haut de la page.
   - Affichage d'une grille de produits avec images, noms et prix.

2. *Filtrage par Catégorie* :
   - Interface utilisateur permettant de sélectionner une catégorie.
   - Mise à jour dynamique des produits affichés en fonction de la catégorie sélectionnée.

3. *Gestion des Favoris* :
   - Icône de cœur pour ajouter ou retirer des produits de la liste des favoris.
   - Indicateur visuel pour montrer si un produit est favori.

### Techniques Illustrées
- *Responsive Design* : L'application s'adapte à différentes tailles d'écran.
- *Gestion des Erreurs* : Traitement des erreurs lors des appels API pour améliorer la robustesse de l'application.

---

Vous pouvez personnaliser cette documentation en fonction de votre style et des détails spécifiques que vous souhaitez inclure. Cela donnera aux utilisateurs et aux développeurs une vue complète de votre projet.
